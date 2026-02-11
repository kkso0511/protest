---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-3/web-drive-3
---

# \[Web, Drive] 파일을 업로드하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 Web 브라우저나 DirectCloud 드라이브를 사용하여 DirectCloud에 파일을 업로드하는 방법에 대해 설명합니다.

***

### 동작 조건

* 이 매뉴얼의 ‘절차’에서는 Shared Box에서의 조작 방법을 설명하고 있지만, Shared Box 이외의 위치에서도 동일한 절차로 작업을 수행할 수 있습니다.
* 파일을 업로드하는 사용자에게는 <마스터>, <전체권한>, <편집자>, <편집자->, <프리뷰어+>, <업로더>의 접근 권한이 부여되어 있어야 합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* [업로드 가능한 파일의 크기를 제한하는 방법](https://help.directcloud.net/admin_manual/undefined/undefined-2)에 따라‘업로드 파일 크기 제한’이 활성화되어 있는 경우, 업로드할 수 있는 파일의 최대 용량은 설정된 값으로 제한됩니다.
* [폴더의 용량 제한을 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-18)의 절차에서 폴더에 저장할 수 있는 파일의 총 용량이 제한되어 있는 경우, 업로드 시 폴더에 포함된 파일 용량의 합계가 제한된 용량을 초과하면\
  “할당 용량을 넘고 있기 때문에 파일을 추가할 수 없습니다.”라는 오류 메시지가 표시되며,\
  초과 이후의 파일은 업로드되지 않습니다.
* 업로드하는 파일 이름에 이전 글꼴의 문자가 포함되어 있으면 일부 문자가 자동으로 새 글꼴로 변환됩니다.
* [워크플로우를 사용하는 방법](https://help.directcloud.net/admin_manual/undefined-7/undefined)에서 워크플로우에 포함되지 않은 ‘결재선 미지정사용자’ 설정의 ‘기능을 제한함’이 선택되어 있는 경우, 워크플로우 신청자로 설정된 사용자 이외에는 폴더 및 파일을 업로드할 수 없습니다.
* DirectCloud AI가 활성화된 폴더에 파일을 업로드하는 경우, 벡터 데이터가 생성됩니다. 벡터 데이터 생성 시에는 파일 내 텍스트 용량 등에 따라 요금이 발생할 수 있으므로 주의가 필요합니다.
* 업로드 대상 폴더에 동일한 이름의 파일이 이미 저장되어 있는 경우, 관리자 페이지의 '반입 정책' 설정에 따라 저장됩니다.\
  단, 아래의 방법으로 파일을 업로드한 경우에는 파일 이름 끝에 자동으로 숫자가 추가됩니다.
  * 링크의 업로드 기능을 이용하여 파일을 업로드
  * 업로드 요청 폴더에 파일을 업로드
  * 업로드 전용 메일을 통해 파일을 업로드
  * Cold Storage에 파일을 업로드
* 파일을 덮어쓰기 저장하면 파일 버전이 갱신됩니다.
* 20MB 이상의 파일을 업로드할 때는 화면 오른쪽 아래의 업로드 알림 화면에서 '×' 버튼을 클릭하여 업로드를 취소할 수 있습니다.
* 20MB 이상의 파일의 업로드에서 네트워크 장애 등의 문제로 업로드가 일시 정지 상태가 된 경우, 아래 절차로 업로드를 재개할 수 있습니다.
  * Web 브라우저:\
    1\. 화면 오른쪽 아래의 업로드 알림 화면을 표시\
    2\. 네트워크 오류가 발생한 파일의 업로드 재개 버튼을 클릭
  * DirectCloud 드라이브:\
    1\. 작업 표시줄에 있는 DirectCloud 드라이브 아이콘을 클릭\
    2\. 상태 탭을 클릭\
    3\. 업로드에 실패한 파일의 오른쪽 또는 화면 하단에 표시되는 “업로드 대기 중인 파일이 ○개 있습니다.”의 재개 아이콘을 클릭
* 업로드를 재개할 수 있는 조건은 업로드 시작 후 12시간 이내이며, 최대 3회까지입니다.\
  업로드 재개에 3회 실패하면 요청되어 있는 모든 업로드가 실패로 처리됩니다.
* 아래의 경우에는 일시 정지된 업로드 재개가 지원되지 않습니다.
  * PC Agent, 모바일 애플리케이션, 모바일용 Web 브라우저, DCMigrator에서의 파일 업로드
  * 워크플로우 승인 기반 업로드, 링크 업로드, 업로드 요청 폴더로의 업로드
* 업로드 진행 중 업로드 대상 경로가 삭제된 경우 업로드는 실패합니다.\
  또한 업로드 대상 폴더가 이동되고 이동된 위치의 상위 폴더 설정에 따라 접근 권한이 제거된 경우에도 업로드는 실패합니다.\
  특히 대용량 파일 업로드로 시간이 오래 걸릴 것으로 예상되는 경우 주의가 필요합니다.
* 업로드가 진행되는 동안 새 URL을 입력하는 등 다른 사이트로 이동하려 하면 Web 브라우저에서 “사이트에서 나갈까요?”라는 확인 메시지가 표시됩니다.\
  “나가기”를 클릭하면 업로드는 중단됩니다
* DirectCloud AI가 활성화된 폴더에 동일한 이름의 파일을 업로드하는 경우의 동작은 다음과 같습니다
  * Web 브라우저에서 파일을 업로드하는 경우 ‘동일한 이름의 파일을 업로드할 때의 처리 방법을 설정하는 방법’의 설정과 관계없이, 파일 이름 끝에 자동으로 ‘-복사본’이 추가되어 별도의 파일로 업로드 됩니다.
  * 링크 업로드 기능, 업로드 요청 폴더, 업로드 전용 메일 주소를 이용해 업로드하는 경우 자동으로 파일 이름 끝에 숫자가 추가되어 별도의 파일로 업로드됩니다.
* DirectCloud-SHIELD IRM을 계약한 경우, 해당 기능이 활성화된 폴더에 기밀 문서 판정 기준에 해당하는 파일이 포함된 폴더를 업로드하면, 업로드된 파일에는 자동으로 기밀도 라벨 및 암호화 설정이 적용됩니다.
* DirectCloud-SHIELD IRM이 활성화된 폴더에서 파일의 기밀도 라벨을 변경하더라도 버전은 갱신되지 않습니다.&#x20;
* DirectCloud에 DirectCloud-SHIELD IRM으로 암호화된 파일은 업로드할 수 없습니다.
* DirectCloud Drive 내에서 파일을 복사하는 경우, PC에 파일이 다운로드된 뒤 복사 대상 폴더로 업로드가 진행되기 때문에, Windows 탐색기 기능만으로는 DirectCloud-SHIELD IRM으로 암호화된 파일을 복사할 수 없습니다.
* 업로드 전용 메일 주소를 통해 파일 업로드 시 발생한 오류는 사용자 페이지에서 확인할 수 없습니다.
* 폴더 트리의 폴더에 폴더를 드래그 앤 드롭하여 폴더 및 파일을 업로드할 때 이미 동일한 이름의 파일이 있는 경우 관리 페이지의 '보안 정책' > '반입 정책'의 '동일명 파일 업로드' 화면에서 처리 방법을 선택해야 합니다.
* 드래그 앤 드롭으로 업로드한 뒤 폴더나 파일이 화면에 표시된 상태로 멈춰 있을 경우, 화면을 새로 고침하십시오.
* Microsoft Access 파일을 클라우드 Storage에 저장하는 것은 권장되지 않습니다.\
  확장자가 ‘accdb’, ‘mdb’인 파일을 DirectCloud에 저장할 경우, 파일이 손상될 위험이 있으므로 주의하십시오.
* 또한 Web 브라우저에서 파일을 다운로드할 때 생성되는 임시 파일(예: .crdownload, .partial 등)은 DirectCloud Drive에 업로드할 수 없습니다.
*   DirectCloud Drive에 파일을 업로드하면 Windows의 다음 폴더에 임시 파일이 생성됩니다. 이 경우 업로드하는 파일과 동일한 하드 디스크 공간이 필요합니다. \
    이 임시 파일은 업로드가 완료될 때까지 보관됩니다.\
    &#xNAN;**`C:\Users\< 사용자 이름>\AppData\Local\DirectCloud Drive\data\< 회사 ID >\< 사용자 >\temp`**\
    <>에 묶인 폴더는 다음과 같이 환경에 따라 변경됩니다.

    <table><thead><tr><th width="153.5" align="center">폴더</th><th align="center">설명</th></tr></thead><tbody><tr><td align="center">＜사용자 이름＞</td><td align="center">Windows의 사용자 이름</td></tr><tr><td align="center">&#x3C; 회사 ID ></td><td align="center">DirectCloud의 회사 ID 시퀀스를 MD5로 일정 길이의 문자열로 해시한 값<br>(예시)<br>820e3ca3-b2b4-ec7d-ec6c-8f74c8da83cd</td></tr><tr><td align="center">&#x3C; 사용자 ></td><td align="center">DirectCloud의 사용자 시퀀스를 MD5로 일정 길이의 문자열로 해시한 값<br>(예시)<br>b21f7f523-975b-3978-1928-ad9009b11b9d</td></tr></tbody></table>
* Windows에서 아이콘을 커스터마이즈한 폴더를 DirectCloud 드라이브에 업로드한 경우, 커스터마이즈된 아이콘은 DirectCloud 드라이브에 반영되지 않습니다.
* DirectCloud 드라이브에서 업로드가 완료되기 전에 네트워크 연결이 끊어진 경우, 다음 절차를 통해 업로드 처리를 재개할 수 있습니다.\
  1\. 작업 표시줄의 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
  2\. \[상태] 탭을 클릭합니다.\
  3\. “업로드 대기 중인 파일이 ○개 있습니다.” 항목에 표시된 재업로드 아이콘을 클릭합니다.
* 또한, Windows의 UNC 경로를 사용하여 DirectCloud 드라이브 애플리케이션 또는 DirectCloud 드라이브의 폴더와 파일을 지정할 수 없습니다.
* iOS 전용 이미지 확장자인 heic, heif 파일을 업로드시, JPEG 파일로 변환하여 업로드합니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 파일 업로드**
{% endhint %}

1. 파일을 업로드할 폴더를 표시합니다.

<figure><img src="../../.gitbook/assets/image (1428).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나로 파일을 업로드합니다.

❶ 상단의 '업로드' 버튼을 클릭하여 파일 선택

<figure><img src="../../.gitbook/assets/image (1429).png" alt=""><figcaption></figcaption></figure>

❷ 드래그 앤 드롭으로 파일 업로드

<figure><img src="../../.gitbook/assets/image (1430).png" alt=""><figcaption></figcaption></figure>



3. 파일이 업로드되었는지 확인합니다.\
   DirectCloud-SHIELD IRM이 활성화된 폴더에 파일을 업로드하는 경우 보안 수준 설정에 따라 업로드된 파일이 암호화되고 확장자가 'irm'으로 변경될 수 있습니다.   \
   또한 '일급 비밀', '기밀' 및 '기밀'과 같은 기밀 유지 라벨이 부여될 수 있습니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-23 153044.png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**업로드 전용 이메일 주소로 파일 업로드**
{% endhint %}

관리자가 업로드 전용 메일 주소를 설정한 경우, 메일에 파일을 첨부하여 전송함으로써 파일을 업로드할 수 있습니다.

1. 메일 프로그램의 수신자란에 관리자가 안내한 메일 주소를 입력하고, 파일을 첨부하여 전송합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-23 153348.png" alt=""><figcaption></figcaption></figure>



2. 파일이 업로드되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-23 153606.png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 파일 업로드**
{% endhint %}

**\[업로드 대상 폴더 보기]**

1. 파일을 업로드할 폴더를 표시합니다.

<figure><img src="../../.gitbook/assets/image (1431).png" alt=""><figcaption></figcaption></figure>



**\[워크플로우가 비활성화된 상태에서 파일 업로드]**

워크플로우가 '사용 안함'으로 설정된 경우, 드래그 앤 드롭으로 파일을 업로드할 수 있습니다.

1. 업로드할 파일을 DirectCloud 폴더로 드래그 앤 드롭합니다.\
   DirectCloud의 폴더에 파일이 복사됩니다.

<figure><img src="../../.gitbook/assets/image (1432).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. PC에 파일을 남기지 않고 DirectCloud로 이동하려면 "Shift" 키를 누른 상태에서 PC의 폴더나 바탕 화면에서 파일을 드래그 앤 드롭합니다.



**\[워크플로우가 활성화된 상태에서 파일 업로드]**

워크플로우를 사용하도록 설정한 경우, 오른쪽 클릭으로 표시되는 메뉴에서 파일 업로드를 신청할 수 있습니다.

1. 파일을 업로드할 폴더를 마우스 오른쪽 버튼으로 클릭하고 표시되는 메뉴에서 'DirectCloud-Drive' > '업로드'를 클릭합니다. 업로드 워크플로우 신청 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1433).png" alt=""><figcaption></figcaption></figure>



2. 워크플로우를 설정하고 신청 버튼을 클릭합니다.\
   신청이 승인되면 파일이 업로드됩니다.

<figure><img src="../../.gitbook/assets/image (1435).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**업로드 알림 이메일 확인**
{% endhint %}

다음 조건을 충족한 상태에서 파일을 업로드하면 <업로더> 접근권한이 부여된 사용자 외에 'Shered Box에 파일이 업로드되었습니다.'라는 제목의 알림 메일이 전송됩니다.

* [특정 폴더에서 업로드 알림 기능을 사용하도록 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-22)
* [알림 메일을 수신할지 여부를 사용자 페이지에서 설정하는 방법](https://help.directcloud.net/user_manual/undefined-13/undefined-3) 의 단계에 따라 '알림 메일'이 '수신됨'으로 설정되어 있습니다.

<figure><img src="../../.gitbook/assets/image (1436).png" alt=""><figcaption></figcaption></figure>
