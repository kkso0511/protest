---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/dcmigrator/limit_speed
---

# DCMigrator의 업로드 속도를 제한하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 사내 파일 서버나 네트워크 하드디스크(NAS)에서 DirectCloud로 데이터를 이전하기 위해 데이터 이전 도구인 DCMigrator를 제공하고 있습니다.\
DCMigrator에서는 Windows PowerShell을 사용하여 파일과 폴더를 DirectCloud로 업로드합니다.\
이 매뉴얼에서는 DCMigrator로 데이터를 이전할 때 업로드 속도를 제한하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼의 제한 사항·추가 설명 및 기본적인 사용 방법에 대해서는 [DCMigrator를 사용하여 데이터를 마이그레이션하는 방법](https://help.directcloud.net/admin_manual/dcmigrator/migration)을 참조해주시기 바랍니다.

***

### 절차

DCMigrator.exe를 실행할 때 JSON 파일을 불러오면 업로드 속도를 조정할 수 있습니다.

{% hint style="warning" %}
**JSON 파일을 생성하기**
{% endhint %}

JSON 파일을 생성한 뒤, 아래 형식에 따라 요일과 시간 단위로 업로드 속도를 설정합니다.

**\[형식]**

<table><thead><tr><th width="120.20001220703125">키</th><th width="84"></th><th width="155.20001220703125"></th><th width="85.20001220703125"></th><th>형</th><th>설명</th></tr></thead><tbody><tr><td>upload_limit</td><td></td><td></td><td></td><td>string</td><td>속도 조정 설정에서 가장 상위에 해당하는 구분입니다.</td></tr><tr><td></td><td>enable</td><td></td><td></td><td>boolean</td><td>업로드 속도 제한 설정을 활성화할지 여부를 지정합니다.<br>true: 활성<br>false: 비활성<br><br><strong>NOTE</strong><br>비활성으로 설정하면 모든 업로드 속도가 자동으로 조정됩니다.</td></tr><tr><td></td><td>default</td><td></td><td></td><td>integer</td><td>요일별/시간별 설정이 지정되지 않은 경우 적용되는 기본 업로드 속도를 설정합니다.<br>0: 자동 속도 조정<br>1~1250: MB 단위로 제한 속도를 지정<br><br><strong>NOTE</strong><br>0 미만 또는 1250을 초과하면 오류가 발생합니다.</td></tr><tr><td></td><td>data</td><td></td><td></td><td>object</td><td>요일별, 시간별 설정 데이터를 정의합니다.</td></tr><tr><td></td><td></td><td>day_of_the_week</td><td></td><td>array_of_strings</td><td><p>단일 또는 여러 요일을 지정합니다(최대 7개).<br>mon: 월요일<br>tue: 화요일<br>wed: 수요일<br>thu: 목요일<br>fri: 금요일<br>sat: 토요일<br>sun: 일요일</p><p>설정 예:<br>["wed", "thu", "fri"]<br></p><p><br><strong>NOTE</strong><br>요일이 중복되면 오류가 발생합니다.</p></td></tr><tr><td></td><td></td><td>time_table</td><td></td><td>array</td><td>시간대별 속도 제한을 지정합니다(최대 4개).<br><br><strong>NOTE</strong><br>5개 이상의 time_table을 지정하면 초과된 설정은 무시됩니다.</td></tr><tr><td></td><td></td><td></td><td>time</td><td>string</td><td><p>시간 범위를 0~24의 숫자로 지정합니다.<br>형식: "시작~종료"</p><p>예1: "0~8"<br>0시 00분~7시 59분 59초</p><p>예2: "8~18"<br>8시 00분~17시 59분 59초<br></p><p><strong>NOTE</strong><br>시간 범위가 겹치면 오류가 발생합니다.</p></td></tr><tr><td></td><td></td><td></td><td>speed</td><td>integer</td><td>업로드 속도 제한값을 MB 단위로 지정합니다.<br>설정값: 1~1250<br><br><strong>NOTE</strong><br>1 미만 또는 1250을 초과하면 오류가 발생합니다.</td></tr></tbody></table>

\
**\[JSON 파일 1]**

* 월, 화\
  0시\~5시는 10MB/s, 5시\~24시는 20MB/s로 제한
* 수, 목, 금\
  1시\~5시는 10MB/s, 5시\~20시는 15MB/s, 20시\~24시는 20MB/s로 제한\
  지정이 없는 0시\~1시는 default 값 0이 적용되어 속도가 자동으로 조정됨
* 토, 일\
  지정이 없기 때문에 default 값 0이 적용되어 속도가 자동으로 조정됨

```
{
    "upload_limit": {
        "enable": true,
        "default": 0,
        "data": [
            {
                "day_of_the_week": [
                    "mon",
                    "tue"
                ],
                "time_table": [
                    {
                        "time": "0~5",
                        "speed": 10
                    },
                    {
                        "time": "5~24",
                        "speed": 20
                    }
                ]
            },
            {
                "day_of_the_week": [
                    "wed",
                    "thu",
                    "fri"
                ],
                "time_table": [
                    {
                        "time": "1~5",
                        "speed": 10
                    },
                    {
                        "time": "5~20",
                        "speed": 15
                    },
                    {
                        "time": "20~24",
                        "speed": 20
                    }
                ]
            }
        ]
    }
}
```



**\[JSON 파일 2]**

월\~금\
0시\~8시는 20MB/s, 8시\~18시는 10MB/s로 제한\
지정이 없는 18시\~24시는 default 값 0이 적용되어 속도가 자동으로 조정됨

토\~일\
0시\~24시는 20MB/s로 제한

```
{
    "upload_limit": {
        "enable": true,
        "default": 0,
        "data": [
            {
                "day_of_the_week": [
                    "mon",
                    "tue",
                    "wed",
                    "thu",
                    "fri"
                ],
                "time_table": [
                    {
                        "time": "0~8",
                        "speed": 20
                    },
                    {
                        "time": "8~18",
                        "speed": 10
                    }
                ]
            },
            {
                "day_of_the_week": [
                    "sat",
                    "sun"
                ],
                "time_table": [
                    {
                        "time": "0~24",
                        "speed": 20
                    }
                ]
            }
        ]
    }
}
```



{% hint style="warning" %}
**속도 조정 JSON을 지정하는 방법**
{% endhint %}

속도 조정 JSON 파일을 불러와 DCMigrator.exe를 실행하는 방법은 두 가지가 있습니다.

\
\[**현재 디렉터리의 JSON 파일을 불러오는 방법]**

명령을 실행하는 디렉터리에 속도 조정 JSON 파일을 저장하여 불러오는 방법입니다.\
JSON 파일 이름은 반드시 "settings.json"으로 저장해야 합니다.

1. 작성한 settings.json 파일을 DCMigrator.exe와 동일한 폴더에 저장합니다.



2. 아래 명령 형식으로 폴더를 업로드하는 명령을 실행합니다.

기타 명령줄 옵션에 대해서는 [DCMigrator를 사용하여 데이터를 마이그레이션하는 방법](https://help.directcloud.net/admin_manual/dcmigrator/migration)의 "DCMigrator의 명령줄 옵션" 항목을 참조해주시기 바랍니다.

명령 형식:

```
DCMigrator.exe "<이전 원본 폴더의 경로>" "/Shared Box/<이전 대상 폴더의 경로>/"
```

실행 예:

```
.\DCMigrator.exe "testfolder" "/Shared Box/mig/testfolder/" ⏎
```

현재 디렉터리에 있는 settings.json 파일이 불러와집니다.



3. 회사 ID(회사코드), 사용자 ID, 비밀번호 입력이 요청되므로 순서대로 입력한 뒤 Enter 키를 누릅니다.

```
Company ID: <회사ID(회사코드)> ⏎
User ID: <사용자ID> ⏎
Password: <비밀번호> ⏎
```

인증에 성공하면, 불러온 JSON 파일에 지정된 속도 조정 설정에 따라 데이터 이전이 시작됩니다.

{% hint style="info" %}
**NOTE**\
JSON 파일이 불러와지면 아래와 같은 Setting 정보가 출력됩니다.
{% endhint %}

```
2025-11-12 18:58:44 INFO Setting : Loaded 'C:\Users\foo\Desktop\settings.json'
```



**\[명령줄 옵션으로 JSON 파일을 지정하는 방법]**

명령줄 옵션 --settings 에 설정 파일의 경로와 JSON 파일 이름을 지정하는 방법입니다.\
이 경우, 현재 디렉터리에 있는 settings.json 파일은 불러와지지 않습니다.

1. 작성한 JSON 파일을 임의의 폴더에 임의의 이름으로 저장합니다.<br>
2.  아래 명령 형식으로 실제 폴더를 업로드하는 명령을 실행합니다.

    기타 명령줄 옵션에 대해서는 DCMigrator를 이용해 데이터를 이전하는 방법의 “DCMigrator의 명령줄 옵션” 항목을 참조해주시기 바랍니다.

명령 형식:

```
DCMigrator.exe "<이전 원본 폴더의 경로>" "/Shared Box/<이전 대상 폴더의 경로>/" --settings="<경로>\settings_group1.json"
```

실행 예:

```
.\DCMigrator.exe "testfolder" "/Shared Box/mig/testfolder/" --settings="C:\Users\foo\Documents\Works\sample\custom_name_settings.json" ⏎
```

지정한 경로에 있는, 지정한 이름의 JSON 파일이 불러와집니다.<br>

3. 회사 ID(회사코드), 사용자 ID, 비밀번호 입력이 요청되므로 순서대로 입력한 뒤 Enter 키를 누릅니다.

```
Company ID: <회사ID(회사코드)> ⏎
User ID: <사용자ID> ⏎
Password: <비밀번호> ⏎
```

인증에 성공하면, 불러온 JSON 파일에 지정된 속도 조정 설정에 따라 데이터 이전이 시작됩니다.

{% hint style="info" %}
**NOTE**\
지정한 JSON 파일이 불러와지면 아래와 같은 Setting 정보가 출력됩니다.
{% endhint %}

```
2025-11-12 18:58:44 INFO Setting : Loaded 'C:\Users\foo\Documents\Works\sample\custom_name_settings.json'
```
