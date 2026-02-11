---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-13/directcloud-2
---

# DirectCloud 드라이브에서 파일 캐시를 활용하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud Drive를 사용할 때 DirectCloud의 파일을 PC에 캐시하도록 설정하면, 용량이 큰 파일을 편집하거나 네트워크 연결이 불안정한 상황에서도 편집 내용을 손상 없이 저장할 수 있습니다.\
이 매뉴얼에서는 DirectCloud Drive에서 파일을 캐시하도록 설정하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 Windows용 DirectCloud Drive의 사양과 절차를 중심으로 설명합니다.\
  macOS용 DirectCloud Drive에서도 동일한 절차로 파일 캐시 사용 여부를 설정할 수 있지만, 일부 기능은 Windows 전용으로 제한되어 있으므로 주의하시기 바랍니다.
* 캐시 기능은 다음 애플리케이션에서 사용할 수 있습니다.
  * DirectCloud Drive(Windows 일반 버전)
  * DirectCloud Drive(macOS 버전)
  * DirectCloud 드라이브(Windows DirectCloud-SHIELD IRM 통합 버전)
  * DirectCloud 드라이브(Windows DirectCloud-SHIELD DLP 통합 버전)
  * DirectCloud 드라이브(macOS 버전)
*   다음의 경우 기본적으로 '캐시 사용 안함'으로 설정됩니다.

    * DirectCloud Drive를 새로 설치한 경우
    * 캐시 기능을 지원하지 않는 버전의 DirectCloud Drive에서 캐시 기능을 지원하는 최신 버전으로 업데이트한 경우

    이 매뉴얼의 절차에 따라 캐시 설정을 활성화한 후 DirectCloud Drive를 버전 업하면, 캐시 설정이 자동으로 이어집니다.
*   캐시 파일은 다음 폴더에 저장됩니다.\
    \
    **Windows:**\
    C:\Users<사용자 이름>\AppData\Local\DirectCloud Drive\data<회사 ID 시퀀스><사용자 시퀀스>\cache<br>

    **macOS:**\
    /Users/<사용자 이름>/Library/Application Support/DirectCloud Drive/data/<회사 ID 시퀀스>/<사용자 시퀀스>/cache<br>

    **<>로 표시된 폴더는 환경에 따라 다음과 같이 달라집니다.**

    <table><thead><tr><th width="173">폴더</th><th>설</th></tr></thead><tbody><tr><td>&#x3C;사용자 이름></td><td>Windows의 사용자 이름 또는 macOS의 사용자 이름</td></tr><tr><td>&#x3C;회사 ID 시퀀스></td><td>DirectCloud의 회사 ID 시퀀스를 MD5로 일정 길이의 문자열로 해시화한 값<br>예: 820e3ca3-b2b4-ec7d-ec6c-8f74c8da83cd</td></tr><tr><td>&#x3C;사용자 시퀀스></td><td>DirectCloud의 사용자 시퀀스를 MD5로 일정 길이의 문자열로 해시화한 값<br>예: b21f7f523-975b-3978-1928-ad9009b11b9d</td></tr></tbody></table>
* 캐시 파일은 다른 사용자와 응용 프로그램이 열 수 없도록 암호화되어 저장됩니다.
* DirectCloud Drive에서 파일을 열 때마다 캐시 파일과 동일한지 여부가 확인됩니다.\
  캐시가 오래된 경우 최신 상태로 캐시 파일이 업데이트됩니다.\
  DirectCloud의 파일과 동일한 경우에는 캐시 파일이 갱신되지 않습니다.
* DirectCloud 드라이브의 파일이 업데이트되면 캐시 파일도 업데이트됩니다.
* 하나의 캐시 파일의 최대 용량은 1GB이며, 1GB를 초과하면 초과한 데이터는 DirectCloud로부터 순차적으로 전송되어 애플리케이션에 반영됩니다.
* 애플리케이션에서 파일을 열면 cache 폴더에 임시로 두 개의 캐시 파일이 생성됩니다. 애플리케이션을 닫으면 임시로 생성된 캐시 파일은 삭제되고, 하나의 캐시 파일로 저장됩니다.
* DirectCloud 드라이브에 저장된 Microsoft Office 파일을 열면 같은 폴더에 '\~$'로 시작하는 임시 파일이 만들어집니다. 또한 위의 <사용자 시퀀스> 폴더 아래의 temp 폴더에도 "\~$"로 시작하는 임시 파일이 만들어집니다. 이 임시 파일은 편집 중인 파일을 닫을 때까지 유지됩니다.
* DirectCloud Drive에서 파일을 업로드할 때는 temp 폴더에 임시 파일이 생성됩니다. 이때 업로드할 파일과 동일한 용량의 하드디스크 공간이 필요합니다. 이 임시 파일은 업로드가 완료될 때까지 유지됩니다.\
  또한 동시에 cache 폴더에 캐시 파일이 생성되며, DirectCloud의 폴더에 파일이 업로드됩니다.
* DirectCloud Drive에서 파일을 덮어쓸 때도 업로드 처리와 동일하게 temp 폴더에 임시 파일이 생성됩니다. 이때 덮어쓸 파일과 동일한 용량의 하드디스크 공간이 필요합니다. 이 임시 파일은 파일을 닫을 때까지 유지됩니다.\
  또한 동시에 cache 폴더의 캐시 파일이 갱신되고, DirectCloud의 파일이 업데이트됩니다.
* temp 폴더에 생성된 임시 파일은 캐시 설정 화면의 캐시 사용 현황에는 포함되지 않습니다.
* 애플리케이션에서 파일을 여는 경우 외에도 다음과 같은 상황에서 캐시 파일이 생성될 수 있습니다.
  * 폴더 내 동일 확장자 데이터를 불러올 때
  * 마우스나 키보드로 포커스를 유지할 때(파일 선택 등)
  * 악성코드 방지 소프트웨어나 파일 검색 프로그램이 파일 데이터를 읽을 때
  * 탐색기나 애플리케이션에서 폴더로 이동하는 과정에서 파일이 호출될 때
* 사용자가 DirectCloud Drive에 로그인한 동안 30초마다 캐시 파일의 최대 개수, 총 용량, 저장 기간이 확인되며, 제한을 초과한 캐시 파일은 자동으로 삭제됩니다.
* 캐시 설정 화면에서 캐시를 삭제하려 할 때 열려 있는 캐시 파일은 사용이 종료된 후에 삭제됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**캐시 설정 화면 표시**
{% endhint %}

1. DirectCloud 드라이브에 로그인합니다.<br>
2. 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (780).png" alt=""><figcaption></figcaption></figure>



3. 설정 화면의 오른쪽 상단에 있는 '⁝' 버튼을 클릭하고 표시된 고급 설정 메뉴에서 캐시 설정을 선택합니다.

<figure><img src="../../.gitbook/assets/image (781).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**캐시를 사용하도록 설정**
{% endhint %}

1. 캐시 설정 화면에서 캐시 사용을 선택합니다.\
   캐시 파일 사용이 활성화되어 PC 디스크의 여유 공간 범위 내에서 DirectCloud 파일이 캐시됩니다.\
   또한 최대 수, 용량 및 보존 기간에 캐시 파일을 제한하려면 2단계로 진행하십시오.

<figure><img src="../../.gitbook/assets/image (782).png" alt=""><figcaption></figcaption></figure>



2. 저장된 캐시 파일을 제한하려면 다음을 설정합니다.

<figure><img src="../../.gitbook/assets/image (783).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="204">항목</th><th>설명</th></tr></thead><tbody><tr><td>캐시 보관 파일 수</td><td><p>캐시 파일 최대 개수 캐시 파일의 개수를 제한하려면 체크박스에 체크하고, 드롭다운 목록에서 캐시 파일의 최대 개수를 선택합니다.<br>저장된 캐시 파일의 총 개수가 여기서 지정한 값을 초과하면 오래된 캐시 파일부터 순서대로 삭제됩니다.<br><br>설정 범위: 10~1000 (50 이상은 50개 단위로 지정)<br></p><p>이 설정을 선택하지 않더라도 캐시 파일의 개수가 5,000개를 초과하면 오래된 캐시 파일부터 자동으로 삭제됩니다.</p></td></tr><tr><td>캐시 용량 제한</td><td>캐시 파일 총 용량 캐시 파일의 용량을 제한하려면 체크박스에 체크하고, 드롭다운 목록에서 캐시 파일의 총 용량을 선택합니다.<br>저장된 캐시 파일의 총 용량이 지정한 값을 초과하면 오래된 캐시 파일부터 순서대로 삭제됩니다.<br><br>설정 범위: 1~100 (5 이상은 5GB 단위로 지정)</td></tr><tr><td>파일 보관기간 제한</td><td><p>캐시 파일 보존 기간 드롭다운 목록에서 캐시 파일을 저장할 일수를 선택합니다.<br><br>설정 범위: 7, 14, 30, 60, 90, 120, 150, 180, 210, 240, 270, 300, 330, 365<br></p><p>파일이 직접 편집, 업로드, 덮어쓰기된 시점부터 설정한 보존 기간이 지나면 캐시 파일은 삭제됩니다.<br>보존 기간이 지나기 전에 파일이 다시 편집, 업로드, 덮어쓰기된 경우 캐시 파일도 갱신되므로, 보존 기간의 계산은 캐시 파일이 갱신된 시점부터 다시 시작됩니다.</p></td></tr></tbody></table>



3. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (784).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**캐시 사용량 확인**
{% endhint %}

저장된 캐시 파일이 있는 경우 다음 단계를 통해 사용 현황을 확인할 수 있습니다. 또한 다음 절차에 따라 캐시를 삭제할 수 있습니다.

1. 캐시 설정 화면의 캐시 사용 현황에서 캐시된 파일의 개수와 용량을 확인합니다.\
   캐시 사용 현황은 사용자가 파일을 수정하거나 삭제한 후 30초 이내에 갱신됩니다.

<figure><img src="../../.gitbook/assets/image (785).png" alt=""><figcaption></figcaption></figure>



2. 캐시를 삭제하려면 캐시 삭제 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (786).png" alt=""><figcaption></figcaption></figure>

&#x20; &#x20;

3. '예' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>

캐시가 삭제되고 '캐시 사용현황'에 '사용된 캐시가 없습니다.'가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (788).png" alt=""><figcaption></figcaption></figure>
