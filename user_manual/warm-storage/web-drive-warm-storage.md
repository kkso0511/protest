---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/warm-storage/web-drive-warm-storage
---

# \[Web, Drive] Warm Storage로 폴더 또는 파일을 이동하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 ‘Warm Storage’를 제공합니다.\
일반적인 Hot Storage에서 링크나 버전 관리 등 일부 기능을 제외한 Warm Storage는 더 저렴한 비용으로 이용할 수 있습니다.\
예를 들어, 자주 사용하지 않는 폴더 계층의 데이터를 모두 Warm Storage로 이동하여 장기 보관하면, Shared Box의 Storage를 효율적으로 활용할 수 있습니다.\
이 매뉴얼에서는 Web 브라우저 및 DirectCloud Drive에서 폴더 또는 파일을 Warm Storage로 이동하는 방법과, 이동한 폴더 또는 파일을 원래의 Hot Storage로 되돌리는 방법에 대해 설명합니다.

***

### 동작조건

* Warm Storage로의 이동을 지원하는 Hot Storage는 Shared Box만 해당됩니다.
* Warm Storage에서는 다음 방향으로 폴더 및 파일을 이동할 수 있습니다.
  * Hot Storage     ➡️ Warm Storage
  * Warm Storage ➡️ Hot Storage
  * Warm Storage ➡️ Warm Storage
* 다음 위치로는 폴더나 파일을 이동할 수 없습니다.
  * Web 브라우저의 'Warm Storage' 메뉴 바로 아래
  * DirectCloud Drive의 'Warm Storage' 폴더 바로 아래
*   Warm Storage에는 폴더 및 파일을 복사하는 기능이 없습니다.\
    따라서 다음 방향으로 폴더 및 파일을 복사할 수 없습니다.

    * Hot Storage     ➡️ Warm Storage
    * Warm Storage ➡️ Hot Storage
    * Warm Storage ➡️ Warm Storage

    Warm Storage에서는 복사가 아닌 이동 기능을 사용해야 합니다.
* 또한 DirectCloud Drive에서는 고스트 기능을 사용할 수 없습니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Warm Storage로 폴더나 파일을 이동하면 다음 정보가 삭제됩니다.
  * **폴더**\
    폴더의 접근 권한\
    폴더 속성
  * **파일**\
    Link History\
    파일 잠금\
    파일 기한
* 파일이나 폴더를 이동하는 사용자는 이동 원본 및 이동 대상 폴더에 적절한 접근 권한이 부여되어 있어야 합니다. 또한, 폴더와 파일 이동에 관한 기본적인 제한 및 보충 사항은 Warm Storage 이외의 폴더에서 이동할 때와 동일합니다.
* Warm Storage에서는 다음 기능을 사용할 수 있습니다.
  * 폴더 생성
  * 업로드
  * 이동
  * 원래 위치로 이동
  * 삭제
  * 이름 변경
  * 즐겨찾기
  * 버전 이력 확인
  * 접근 이력
  * 미리보기 (유료 옵션)
  * 다운로드 (유료 옵션)
  * 전체 검색 (유료 옵션)
* DirectCloud 드라이브 에서는 업로드 권한이 있는 사용자도 warm storage 폴더에 파일을 바로 업로드 할 수 없습니다. Shared Box에서 warm storage로 이동 기능을 사용해 주시거나, web 브라우저에서 업로드 부탁드립니다.
* 사용자 페이지의 Warm Storage 폴더 속성에서는 '자동 삭제', '버전 관리', '승인 워크플로우', 'SHIELD', '업로드 전용 메일 주소', '메일 알림', '링크', '코멘트'가 표시되지 않습니다.

***

### 절차

{% hint style="warning" %}
**Web 브라우저에서 Warm Storage 사용**
{% endhint %}

이 매뉴얼에서는 Shared Box의 폴더 또는 파일을 Warm Storage로 이동하는 방법에 대해 설명합니다.

1. Shared Box 아래의 폴더에서 Warm Storage로 이동하려는 폴더 또는 파일에 체크하고 '이동' 버튼을 클릭합니다.\
   여러 개의 폴더와 파일을 동시에 선택할 수도 있습니다.\
   마우스 오른쪽 버튼을 클릭해 표시되는 메뉴나 오른쪽의 ▼ 버튼을 클릭해 나타나는 메뉴에서 '이동'을 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (2199).png" alt=""><figcaption></figcaption></figure>



2. 이동할 폴더에서 'Warm Storage' 아래의 폴더를 선택하고 '이동' 버튼을 클릭합니다.\
   '새 폴더'를 클릭하여 이동할 폴더를 새로 생성할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (2200).png" alt=""><figcaption></figcaption></figure>



3. 이동을 진행해도 되는 경우 '확인' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2201).png" alt=""><figcaption></figcaption></figure>



4. Warm Storage로 이동된 폴더나 파일의 고스트가 표시되어 있는지 확인합니다.\
   고스트는 복사하거나 이동할 수는 없지만, 고스트를 이용하여 이동된 위치의 정보를 확인하거나 이동한 폴더 및 파일을 되돌릴 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2203).png" alt=""><figcaption></figcaption></figure>



**\[Warm Storage로 이동된 파일 확인]**

1. Warm Storage의 폴더에서 Shared Box에서 이동된 폴더 또는 파일을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2204).png" alt=""><figcaption></figcaption></figure>

* Shared Box에서 이동된 폴더나 파일의 아이콘에는 배지가 표시됩니다.
* Warm Storage로 이동한 폴더에 하위 폴더나 파일이 포함되어 있는 경우, 하위 폴더나 파일의 아이콘에는 배지가 표시되지 않습니다.
* 배지의 색상은 폴더나 파일을 원래 위치로 되돌릴 때의 위치에 따라 달라집니다.

<table><thead><tr><th width="128">배지색상</th><th>설명</th></tr></thead><tbody><tr><td>빨간색</td><td>Warm Storage로 이동되기 전에 저장되어 있던 폴더가 Shared Box에 있는 경우</td></tr><tr><td>주황색</td><td>Warm Storage로 이동되기 전에 저장되어 있던 폴더가 Warm Storage로 이동된 경우</td></tr></tbody></table>



2. 배지가 표시된 폴더 또는 파일 아이콘에 커서를 올립니다.\
   툴팁에 이동 원본 폴더 또는 파일의 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2205).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="127">항목</th><th>설명</th></tr></thead><tbody><tr><td>위치</td><td>Warm Storage로 이동된 폴더 또는 파일이 이동되기 전에 저장되어 있던 폴더의 폴더 경로가 표시됩니다.<br>이동 원본 폴더가 다시 이동되면 폴더 경로도 함께 변경됩니다.<br>Warm Storage에서 Shared Box로 폴더 또는 파일을 되돌릴 때 ‘원래 위치로 이동’을 선택하면, 이 폴더 경로 아래로 이동됩니다.</td></tr><tr><td>이동날짜</td><td>Warm Storage로 처음 이동된 날짜와 시간이 표시됩니다.</td></tr><tr><td>사용자이름</td><td>폴더 또는 파일을 이동한 사용자의 이름과 사용자 ID, 그리고 이동 방식(‘수동 이동’ 또는 ‘자동 이동’)이 표시됩니다.</td></tr></tbody></table>



**\[Warm Storage에서 Shared Box로 폴더 또는 파일을 복원]**

Warm Storage로 이동된 폴더 또는 파일을 Shared Box의 원래 폴더로 되돌리는 방법에 대해 설명합니다.

1. Warm Storage에서 Shared Box로 되돌리고자 하는 폴더 또는 파일을 표시합니다.

<figure><img src="../../.gitbook/assets/image (2204).png" alt=""><figcaption></figcaption></figure>



2. 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하거나 오른쪽의 ▼ 버튼을 클릭한 뒤, 표시된 메뉴에서 '원위치 이동'을 선택합니다.\
   여러 개의 폴더와 파일을 동시에 선택하여 되돌릴 수는 없습니다.

<figure><img src="../../.gitbook/assets/image (2206).png" alt=""><figcaption></figcaption></figure>

폴더 또는 파일이 Shared Box의 원래 폴더로 이동되며, ‘원래 위치로 이동이 완료되었습니다.’라는 메시지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2207).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 Warm Storage 사용**
{% endhint %}

**\[폴더 또는 파일을 Warm Storage로 이동하기]**

이 매뉴얼에서는 Shared Box의 폴더 또는 파일을 Warm Storage로 이동하는 방법에 대해 설명합니다.

1. Shared Box 아래의 폴더에서 Warm Storage로 이동하려는 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 ‘DirectCloud-Drive’ > ‘Warm Storage로 이동’을 클릭합니다.\
   여러 개의 폴더와 파일을 동시에 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (2208).png" alt=""><figcaption></figcaption></figure>



2. 이동할 Warm Storage의 폴더를 선택하고 '이동' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2209).png" alt="" width="563"><figcaption></figcaption></figure>



3. 이동을 진행해도 되는 경우 '확인' 버튼을 클릭합니다

<figure><img src="../../.gitbook/assets/image (2210).png" alt="" width="563"><figcaption></figcaption></figure>



**\[Warm Storage로 이동된 폴더와 파일을 확인하기]**

DirectCloud Drive의 경우, Shared Box에서 이동된 폴더나 파일에는 배지가 표시되지 않습니다.\
이 매뉴얼에서는 Shared Box에서 이동된 폴더나 파일의 정보를 확인하는 방법에 대해 설명합니다.

1. Warm Storage의 폴더에서 Shared Box에서 이동된 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 ‘DirectCloud Drive’ > ‘원위치 정보’을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2211).png" alt=""><figcaption></figcaption></figure>

&#x20;     이동 원본 폴더 또는 파일의 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2212).png" alt="" width="375"><figcaption></figcaption></figure>

<table><thead><tr><th width="127">항목</th><th>설명</th></tr></thead><tbody><tr><td>위치</td><td>Warm Storage로 이동된 폴더 또는 파일이 이동되기 전에 저장되어 있던 폴더의 폴더 경로가 표시됩니다.<br>이동 원본 폴더가 다시 이동되면 폴더 경로도 함께 변경됩니다.<br>Warm Storage에서 Shared Box로 폴더 또는 파일을 되돌릴 때 ‘원래 위치로 이동’을 선택하면, 이 폴더 경로 아래로 이동됩니다.</td></tr><tr><td>이동날짜</td><td>Warm Storage로 처음 이동된 날짜와 시간이 표시됩니다.</td></tr><tr><td>사용자이름</td><td>폴더 또는 파일을 이동한 사용자의 이름과 사용자 ID, 그리고 이동 방식(‘수동 이동’ 또는 ‘자동 이동’)이 표시됩니다.</td></tr></tbody></table>

\
**\[Warm Storage에서 Shared Box로 폴더 또는 파일을 되돌리기]**

Warm Storage로 이동된 폴더 또는 파일을 Shared Box의 원래 폴더로 되돌리는 방법에 대해 설명합니다.

1. Warm Storage에서 Shared Box로 되돌리고자 하는 폴더 또는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 ‘DirectCloud Drive’ > ‘원래 위치로 이동’을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2211).png" alt=""><figcaption></figcaption></figure>

&#x20;      폴더 또는 파일이 Shared Box의 원래 폴더로 이동합니다.
