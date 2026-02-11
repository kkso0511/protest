---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-3/ghost
---

# 사용자 페이지에서 Ghost(고스트) 파일을 조작하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 Warm Storage를 제공합니다.\
일반 Hot Storage에서 링크나 버전 관리 등의 일부 기능을 제외한 Warm Storage는 보다 저렴한 비용으로 이용할 수 있습니다.\
예를 들어, 자주 사용하지 않는 폴더 계층의 데이터를 전체적으로 Warm Storage로 이동하여 장기 보관함으로써, Shared Box의 Storage를 효율적으로 활용할 수 있습니다.\
이 매뉴얼에서는 사용자 페이지에서 Warm Storage로 이동된 파일의 고스트를 조작하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Warm Storage를 사용할 수 있는경우, 사용자 페이지에 ‘Warm Storage’ 메뉴가 표시됩니다.
* 고스트를 이용하여 폴더나 파일을 이동하려면, 이동 원본 및 이동 대상 폴더 모두에 적절한 접근 권한이 부여되어 있어야 합니다. 또한 폴더와 파일 이동에 관한 기본적인 제한 및 보충 사항은 Warm Storage 외의 폴더에서 이동할 때와 동일합니다.\
  자세한 내용은 아래의 제한·보충 사항을 참고해 주십시오.
  * [\[Web, Drive\] 폴더를 이동하는 방법](https://help.directcloud.net/user_manual/undefined-1/web-drive-1)
  * [\[Web, Drive\] 파일을 이동하는 방법](https://help.directcloud.net/user_manual/undefined-3/web-drive-5)
* 관리자가 고스트 기능을 ‘사용하지 않음’으로 설정한 경우, 고스트는 표시되지 않습니다.\
  관리자 페이지 중 '공유 설정'->'세부 기능 설정'->'Warm Storage로 이동한 흔적 표시' 에서 설정 가능합니다.
* 고스트는 다른 폴더로 이동할 수 없습니다.
* 고스트는 폴더나 파일의 실제 데이터가 아니기 때문에, 고스트와 동일한 폴더 내에 같은 이름의 폴더나 파일을 업로드, 이동 또는 복사할 수 있습니다.\
  단, 동일한 이름의 폴더나 파일이 이미 존재하는 경우, 해당 고스트로부터 원래 파일을 되돌릴 수는 없습니다.
* Warm Storage로 이동된 폴더나 파일의 이름이 변경되거나 다른 위치로 이동된 경우, 그 내용은 고스트에도 반영됩니다.
* Warm Storage로 이동된 폴더나 파일이 삭제되면, 고스트도 함께 삭제됩니다.
* Warm Storage로 이동된 폴더나 파일을 Warm Storage 이외의 폴더로 이동한 경우, 고스트는 다음과 같이 처리됩니다.
  * 이동 원본이 아닌 Shared Box로 이동한 경우: 고스트는 삭제됩니다.
  * Shared Box 이외의 폴더로 이동한 경우: 고스트는 삭제되지 않으며, 고스트의 “저장 위치” 정보가 변경됩니다.
* 고스트는 사용자 또는 관리자의 휴지통으로 이동되지 않으므로, 한 번 삭제되면 복원할 수 없습니다.
* 또한 ‘비즈니스’ 이상 요금제에서 유료 옵션인 Cold Storage를 계약한 경우, 사용자 페이지에 ‘Cold Storage’ 메뉴가 표시됩니다.
* Warm Storage에 저장된 파일을 Cold Storage로 이동하면, 해당 고스트는 삭제되며, 고스트를 이용하여 Shared Box나 Warm Storage로 되돌릴 수 없게 됩니다.

***

### 절차

{% hint style="warning" %}
**Ghost(고스트)란 무엇인가요?**
{% endhint %}

고스트란, Shared Box 내의 폴더 또는 파일이 Warm Storage로 이동되었을 때, 이동 원본 위치에 표시되는 정보를 말합니다.\
고스트는 흐릿한 색상으로 표시되며, 아이콘의 오른쪽 하단에는 Warm Storage 배지가 함께 표시됩니다.\
![](<../../.gitbook/assets/image (2442).png>)

고스트는 이동된 대상 위치, 이동 일시, 이동한 사용자 등의 정보만을 보유하고 있습니다.\
폴더나 파일의 실제 데이터가 아니므로, 클릭하여 폴더로 이동하거나 파일을 열람할 수 없으며, 체크박스로 선택하는 것도 불가능합니다.

또한, 본 매뉴얼의 '고스트 삭제하기' 절차를 통해 고스트를 삭제할 수 있지만, 이 경우에도 이동된 대상 폴더나 파일의 실제 데이터는 삭제되지 않습니다.



{% hint style="warning" %}
**Ghost에서 폴더 또는 파일의 저장 위치 확인하기**
{% endhint %}

1. 폴더 또는 파일의 Ghost 아이콘에 커서를 올립니다.\
   Warm Storage로 이동된 폴더 또는 파일의 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2443).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="166.79998779296875" align="center">항목</th><th>설명</th></tr></thead><tbody><tr><td align="center">보관 위치</td><td>Ghost의 실제 폴더 또는 파일이 저장되어 있는 폴더 경로가 표시됩니다.</td></tr><tr><td align="center">이동날짜</td><td>Ghost의 실제 폴더 또는 파일이 처음 Warm Storage로 이동된 날짜와 시간이 표시됩니다.</td></tr><tr><td align="center">사용자 이름</td><td>폴더 또는 파일을 이동한 사용자 이름과 사용자 ID, 그리고 이동 방식(수동 이동 또는 자동 이동)이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**Ghost에서 Warm Storage로 이동**
{% endhint %}

1. Shared Box 에서폴더 또는 파일의 고스트를 마우스 오른쪽 버튼으로 클릭하거나, 오른쪽의 ▼ 버튼을 클릭한 후 표시된 메뉴에서 ‘보관위치로 이동’을 선택합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 085647 (1).png" alt=""><figcaption></figcaption></figure>

Warm Storage의 폴더에 고스트의 실제 폴더 또는 파일이 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 085935.png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**고스트에서 Warm Storage의 폴더 및 파일을 Shared Box로 되돌리기**
{% endhint %}

Warm Storage로 이동된 폴더 또는 파일은, 고스트가 있는 폴더에서 ‘이동’을 통해 원래 위치로 되돌릴 수 있습니다.

1. 폴더 또는 파일의 고스트를 마우스 오른쪽 버튼으로 클릭하거나, 오른쪽의 ▼ 버튼을 클릭한 후 표시된 메뉴에서 ‘이동으로 가져오기’를 선택합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 091519.png" alt=""><figcaption></figcaption></figure>

선택한 폴더 또는 파일이 Warm Storage에서 이동되어 고스트가 사라집니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 091645.png" alt=""><figcaption></figcaption></figure>



2. Warm Storage에서 이동으로 되돌린 폴더 또는 파일이 삭제되었는지 확인합니다.



{% hint style="warning" %}
**고스트 제거**
{% endhint %}

아래의 절차로 고스트를 삭제하면, Warm Storage로 이동된 폴더나 파일은 고스트에서 조작할 수 없게 됩니다.

1. 폴더 또는 파일의 고스트를 마우스 오른쪽 버튼으로 클릭하거나, 오른쪽의 ▼ 버튼을 클릭하여 표시된 메뉴에서 '삭제'를 선택합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 092247.png" alt=""><figcaption></figcaption></figure>

고스트가 삭제 됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 092359.png" alt=""><figcaption></figcaption></figure>



2. Warm Storage에서 고스트를 삭제한 폴더 또는 파일을 확인하고, 아이콘에서 배지가 삭제된 것을 확인합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-10-24 092447.png" alt=""><figcaption></figcaption></figure>

