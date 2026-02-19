---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_management/wd_move_to_warm
---

# \[Web, Drive] Warm Storage로 폴더 또는 파일을 이동하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 Warm Storage를 제공합니다.\
일반 Hot Storage에서 링크나 버전 관리 등의 일부 기능을 제외한 Warm Storage는 보다 저렴한 비용으로 이용할 수 있습니다.\
예를 들어, 자주 사용하지 않는 폴더 계층의 데이터를 전체적으로 Warm Storage로 이동하여 장기 보관함으로써, Shared Box의 Storage를 효율적으로 활용할 수 있습니다.\
이 매뉴얼에서는, Web 브라우저 및 DirectCloud 드라이브에서 Warm Storage로 폴더 또는 파일을 이동하는 방법과, 이동한 폴더 또는 파일을 원래의 Hot Storage로 되돌리는 방법에 대해 설명합니다.

***

### 작동조건 <a href="#a04" id="a04"></a>

* Warm Storage로 이동할 수 있는 Hot Storage는 Shared Box만 해당됩니다.
* Warm Storage에서는 폴더와 파일을 다음과 같은 방향으로 이동할 수 있습니다.
  * Hot Storage → Warm Storage
  * Warm Storage → Hot Storage
  * Warm Storage → Warm Storage
* 다음 위치로 폴더나 파일을 이동할 수는 없습니다.
  * Web 브라우저의 'Warm Storage' 메뉴 바로 아래
  * DirectCloud 드라이브의 'Warm Storage' 폴더 바로 아래
* Warm Storage에는 폴더 및 파일을 복사하는 기능이 없습니다. 따라서 다음 방향으로 폴더나 파일을 복사할 수 없습니다.
  * Hot Storage → Warm Storage
  * Warm Storage → Hot Storage
  * Warm Storage → Warm Storage
* Warm Storage에서는 복사 대신 이동을 사용해야 합니다.\
  또한, DirectCloud 드라이브에서는 Ghost 기능을 사용할 수 없습니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Warm Storage로 폴더나 파일을 이동하면 다음 정보가 삭제됩니다.\
  **폴더:** 폴더의 접근 권한, 폴더 속성 \
  **파일:** 링크 이력, 파일 잠금, 파일 만료일
* 폴더나 파일을 이동하는 사용자에게는 이동 전후 폴더에 적절한 접근 권한이 부여되어 있어야 합니다.\
  또한, 폴더 및 파일 이동에 대한 기본적인 제한 사항과 보충 사항은, Warm Storage 외 폴더에서 이동할 때와 동일합니다.
* Warm Storage에서는 다음 기능을 이용할 수 있습니다.\
  · 폴더 생성\
  · 업로드\
  · 이동\
  · 원래 위치로 이동\
  · 삭제\
  · 이름 변경\
  · 즐겨찾기\
  · 버전 이력 확인\
  · 접근 이력\
  · 미리보기\
  · 다운로드\
  · 전체 검색
* 사용자 페이지의 Warm Storage 폴더 속성에는 다음 항목이 표시되지 않습니다.\
  · 자동 삭제\
  · 버전 관리\
  · 워크플로우\
  · SHIELD\
  · 업로드 전용 메일 주소\
  · 메일 알림\
  · 링크\
  · 코멘트

***

### 절차

{% hint style="warning" %}
**Web 브라우저에서 Warm Storage 활용**
{% endhint %}

**\[폴더 또는 파일을 Warm Storage로 이동]**

Shared Box의 폴더나 파일을 Warm Storage로 이동하는 방법은 다음과 같습니다.<br>

1.  Shared Box 아래의 폴더에서 Warm Storage로 이동하려는 폴더 또는 파일에 체크를 하고, '이동' 버튼을 클릭합니다.\
    여러 개의 폴더와 파일을 동시에 선택할 수 있습니다.

    또한, 마우스 오른쪽 버튼 클릭으로 표시되는 메뉴나 오른쪽의 ▼ 버튼을 클릭하여 표시된 메뉴에서 '이동'을 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 080135.png" alt=""><figcaption></figcaption></figure>



2. 이동할 대상 폴더로 'Warm Storage'아래의 폴더를 선택하고, '이동'버튼을 클릭합니다.\
   '새 폴더'를 클릭하여 이동할 폴더를 새로 생성할 수도 있습니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 080234.png" alt=""><figcaption></figcaption></figure>



3. 이동하려면 확인 버튼을 클릭합니다.\
   선택한 폴더 또는 파일이 Warm Storage로 이동합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 080410.png" alt=""><figcaption></figcaption></figure>



4. Warm Storage로 이동된 폴더와 파일의 Ghost가 표시되는 것을 확인합니다.\
   Ghost는 복사하거나 이동할 수 없지만, Ghost를 이용하여 이동 대상 정보를 확인하거나, 이동한 폴더와 파일을 되돌릴 수 있습니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 080520.png" alt=""><figcaption></figcaption></figure>



**\[Warm Storage로 이동된 폴더 및 파일 확인]**

1. Warm Storage 폴더에서 Shared Box 폴더에서 이동된 폴더 또는 파일을 봅니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 080617.png" alt=""><figcaption></figcaption></figure>

* Shared Box에서 이동된 폴더와 파일의 아이콘에는 배지가 표시됩니다.
* Warm Storage로 이동한 폴더에 하위 폴더나 파일이 포함된 경우, 하위 폴더와 파일의 아이콘에는 배지가 표시되지 않습니다.
*   배지의 색상은 폴더나 파일을 원래 위치로 되돌릴 때의 위치에 따라 달라집니다.

    <table><thead><tr><th width="182">색상</th><th>설명</th></tr></thead><tbody><tr><td>빨간색</td><td>Warm Storage로 이동되기 전에 Shared Box에 저장되어 있었던 경우</td></tr><tr><td>주황색</td><td>Warm Storage로 이동되기 전에 Warm Storage에 저장되어 있었던 경우</td></tr></tbody></table>



2. 배지가 표시되는 폴더 또는 파일의 아이콘 위로 마우스를 가져갑니다.\
   도구 설명에는 이동하려는 폴더 또는 파일에 대한 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 080733 (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="156">항목</th><th>설명</th></tr></thead><tbody><tr><td>위치</td><td>Warm Storage로 이동된 폴더 또는 파일이 이동되기 전에 저장되어 있던 폴더의 폴더 경로가 표시됩니다.<br>이동 전 폴더 자체가 이동되면 해당 폴더 경로도 함께 변경됩니다.<br>Warm Storage에서 Shared Box로 폴더 또는 파일을 되돌릴 때 "원래 위치로 이동"을 선택하면, 이 폴더 경로 아래로 이동됩니다.</td></tr><tr><td>이동날짜</td><td>Warm Storage로 처음 이동된 날짜와 시간이 표시됩니다.</td></tr><tr><td>사용자</td><td>폴더 또는 파일을 이동시킨 사용자의 이름과 사용자 ID, 그리고 이동 방식(수동 이동 또는 자동 이동)이 표시됩니다.</td></tr></tbody></table>



**\[Warm Storage에서 Shared Box로 폴더 또는 파일 반환]**

Warm Storage로 이동된 폴더 또는 파일을 Shared Box의 원래 폴더로 되돌리는 방법에 대해 설명합니다.

1. Warm Storage에서 Shared Box로 되돌리고 싶은 폴더 또는 파일을 표시합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 080617 (1).png" alt=""><figcaption></figcaption></figure>



2. 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하거나, 오른쪽의 ▼ 버튼을 클릭하여 표시된 메뉴에서 '원위치 이동'을 선택합니다.\
   여러 개의 폴더와 파일을 동시에 되돌릴 수는 없습니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 081554.png" alt=""><figcaption></figcaption></figure>



3. 폴더 또는 파일이 Shared Box의 원래 폴더로 이동되면, "원위치로 이동이 완료되었습니다."라는 메시지가 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 081654.png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 Warm Storage 사용**
{% endhint %}

**\[폴더 또는 파일을 Warm Storage로 이동]**

Shared Box의 폴더나 파일을 Warm Storage로 이동하는 방법은 다음과 같습니다.

1. Shared Box 아래의 폴더에서 Warm Storage로 이동할 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 'DirectCloud-Drive' > 'Warm Storage로 이동'을 클릭합니다.\
   여러 개의 폴더와 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 081814.png" alt=""><figcaption></figcaption></figure>



2. 이동하려는 Warm Storage 폴더를 선택하고 이동 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 081910.png" alt=""><figcaption></figcaption></figure>



3. 이동하려면 OK 버튼을 클릭합니다.\
   선택한 폴더 또는 파일이 Warm Storage로 이동합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 082033.png" alt=""><figcaption></figcaption></figure>



**\[Warm Storage로 이동된 폴더 및 파일 확인]**

DirectCloud 드라이브의 경우, Shared Box에서 이동된 폴더 또는 파일에는 배지가 표시되지 않습니다.\
여기서는 Shared Box에서 이동된 폴더 또는 파일의 정보를 확인하는 방법에 대해 설명합니다.

1. Warm Storage 폴더에서 Shared Box에서 이동된 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 'DirectCloud-Drive' > '원위치 정보'을 클릭합니다.\
   이동하려는 폴더 또는 파일의 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 0821581.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 082251.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="134">항목</th><th>설명</th></tr></thead><tbody><tr><td>위치</td><td>Warm Storage로 이동된 폴더 또는 파일이 이동되기 전에 저장되어 있던 폴더의 경로가 표시됩니다. 이동 전 폴더가 이동되면 해당 경로도 함께 변경됩니다.<br>Warm Storage에서 Shared Box로 폴더 또는 파일을 되돌릴 때 ‘원래 위치로 이동’을 선택하면, 이 경로 아래로 이동됩니다.</td></tr><tr><td>이동날짜</td><td>이동 일시 Warm Storage로 처음 이동된 날짜와 시간이 표시됩니다.</td></tr><tr><td>사용자</td><td>사용자명 폴더 또는 파일을 이동시킨 사용자 이름과 사용자 ID, 그리고 이동 방식(수동 이동 또는 자동 이동)이 표시됩니다.</td></tr></tbody></table>



**\[Warm Storage에서 공유 폴더로 폴더 또는 파일 반환]**

폴더 또는 파일을 Shared Box의 원래 폴더로 다시 이동하는 방법에 대해 설명합니다.

1. Warm Storage에서 Shared Box로 되돌리고 싶은 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 'DirectCloud-Drive' > '원위치 이동'을 클릭합니다.\
   폴더 또는 파일이 공유 폴더의 원래 폴더로 이동됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 082158.png" alt=""><figcaption></figcaption></figure>
