---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/warm-storage/use_ghost
---

# 사용자 페이지에서 고스트(Ghost)를 조작하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 ‘Warm Storage’를 제공합니다.\
일반적인 Hot Storage에서 링크나 버전 관리 등 일부 기능을 제외한 Warm Storage는 더 저렴한 비용으로 이용할 수 있습니다.\
예를 들어, 자주 사용하지 않는 폴더 계층의 데이터를 모두 Warm Storage로 이동하여 장기 보관하면, Shared Box의 Storage를 효율적으로 활용할 수 있습니다.\
이 매뉴얼에서는 사용자 페이지에서 Warm Storage로 이동된 파일의 고스트를 조작하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Warm Storage를 이용할 수 있는 경우, 사용자 페이지에 ‘Warm Storage’ 메뉴가 표시됩니다.
* 고스트를 조작하여 파일이나 폴더를 이동하는 사용자는 이동 원본 및 이동 대상 폴더에 적절한 접근 권한이 부여되어 있어야 합니다.\
  또한 폴더와 파일 이동에 관한 기본적인 제한 및 보충 사항은 Warm Storage 이외의 폴더에서 이동할 때와 동일합니다.
* 관리자 페이지에서 '공유설정'->'세부 기능 설정'->'Warm Storage로 이동한 흔적 표시' 항목이 사용 안함 으로 되어있다면 고스트가 표시되지 않습니다.
* 고스트는 다른 폴더로 이동할 수 없습니다.
* 고스트는 폴더나 파일의 실제 데이터가 아니기 때문에, 동일한 폴더 안에 고스트와 같은 이름의 폴더나 파일을 업로드·이동·복사할 수 있습니다.\
  그러나 고스트로부터 동일한 이름의 폴더나 파일을 되돌릴 수는 없습니다.
* Warm Storage로 이동된 폴더나 파일의 이름이 변경되거나 이동된 경우, 그 내용은 고스트에도 반영됩니다.
* Warm Storage로 이동된 폴더나 파일이 삭제되면, 고스트 또한 함께 삭제됩니다.
* Warm Storage로 이동된 폴더나 파일을 Warm Storage 이외의 다음 폴더로 이동한 경우, 고스트의 상태는 다음과 같습니다.
  * 이동 원본이 아닌 Shared Box로 이동한 경우:\
    고스트는 삭제됩니다.
  * Shared Box 이외의 폴더로 이동한 경우:\
    고스트는 삭제되지 않으며, 고스트의 ‘저장 위치’ 정보가 변경됩니다.
* 고스트는 사용자 휴지통이나 관리자 휴지통으로 이동되지 않기 때문에, 한 번 삭제되면 복원할 수 없습니다.
* Cold Storage를 계약한 경우, 사용자 페이지에 ‘Cold Storage’ 메뉴가 표시됩니다.
* Warm Storage에 저장된 파일을 Cold Storage로 이동하면 고스트가 삭제되며, 고스트를 이용해 Shared Box나 Warm Storage로 되돌릴 수 없게 됩니다.

***

### 절차

{% hint style="warning" %}
**고스트(Ghost)란?**
{% endhint %}

Shared Box의 폴더 및 파일이 Warm Storage로 이동되었을 때, 이동 원래 위치에 표시되는 정보를 ‘고스트’라고 합니다.\
고스트는 옅은 색으로 표시되며, 아이콘의 오른쪽 아래에는 Warm Storage 배지가 표시됩니다.

* 사용자 페이지에서의 고스트 표시 예(폴더)\
  ![](<../../.gitbook/assets/image (421).png>)
*   사용자 페이지에서의 고스트 표시 예(파일)

    <div align="left"><figure><img src="../../.gitbook/assets/image (420).png" alt="" width="207"><figcaption></figcaption></figure></div>

고스트는 이동 위치, 이동 일시, 이동한 사용자 등의 정보만을 가지고 있습니다.\
폴더나 파일의 실제 데이터가 아니기 때문에, 클릭하여 폴더로 이동하거나 파일을 열어볼 수 없습니다. 또한 체크박스로 선택하는 것도 불가능합니다.\
이 매뉴얼의 ‘고스트를 삭제하기’ 절차를 통해 고스트를 삭제할 수 있지만, 그로 인해 이동된 폴더나 파일이 삭제되는 것은 아닙니다.



{% hint style="warning" %}
**고스트에서 폴더 또는 파일의 저장 위치를 확인하기**
{% endhint %}

1. 폴더 또는 파일의 고스트 아이콘에 커서를 올립니다.\
   Warm Storage로 이동된 폴더 또는 파일의 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2205).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="127">항목</th><th>설명</th></tr></thead><tbody><tr><td>위치</td><td>Warm Storage로 이동된 폴더 또는 파일이 이동되기 전에 저장되어 있던 폴더의 폴더 경로가 표시됩니다.<br>이동 원본 폴더가 다시 이동되면 폴더 경로도 함께 변경됩니다.<br>Warm Storage에서 Shared Box로 폴더 또는 파일을 되돌릴 때 ‘원래 위치로 이동’을 선택하면, 이 폴더 경로 아래로 이동됩니다.</td></tr><tr><td>이동날짜</td><td>Warm Storage로 처음 이동된 날짜와 시간이 표시됩니다.</td></tr><tr><td>사용자이름</td><td>폴더 또는 파일을 이동한 사용자의 이름과 사용자 ID, 그리고 이동 방식(‘수동 이동’ 또는 ‘자동 이동’)이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**고스트에서 Warm Storage의 저장 위치로 이동하기**
{% endhint %}

1. 폴더 또는 파일의 고스트를 마우스 오른쪽 버튼으로 클릭하거나, 오른쪽의 ▼ 버튼을 클릭한 뒤 표시된 메뉴에서 ‘저장 위치로 이동’을 선택합니다.

<figure><img src="../../.gitbook/assets/image (423).png" alt=""><figcaption></figcaption></figure>

&#x20;      Warm Storage의 폴더에 고스트의 실제 폴더 또는 파일이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (424).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**고스트에서 Warm Storage의 폴더 및 파일을 Shared Box로 되돌리기**
{% endhint %}

Warm Storage로 이동된 폴더 또는 파일은 고스트가 있는 폴더로 ‘이동’을 통해 되돌릴 수 있습니다.

1. 폴더 또는 파일의 고스트를 마우스 오른쪽 버튼으로 클릭하거나 오른쪽의 ▼ 버튼을 클릭한 뒤, 표시된 메뉴에서 ‘이동으로 가져오기’를 선택합니다.

<figure><img src="../../.gitbook/assets/image (425).png" alt=""><figcaption></figcaption></figure>

&#x20;     선택한 폴더 또는 파일이 Warm Storage에서 이동되며, 고스트가 사라집니다.

<figure><img src="../../.gitbook/assets/image (426).png" alt=""><figcaption></figcaption></figure>

2. Warm Storage에서 ‘이동으로 되돌리기’를 수행한 폴더 또는 파일이 삭제된 것을 확인합니다.



{% hint style="warning" %}
**고스트를 삭제하기**
{% endhint %}

아래 절차로 고스트를 삭제하면, Warm Storage로 이동된 폴더나 파일은 고스트를 통해 조작할 수 없게 됩니다.

1. 폴더 또는 파일의 고스트를 마우스 오른쪽 버튼으로 클릭하거나, 오른쪽의 ▼ 버튼을 클릭한 뒤 표시된 메뉴에서 ‘삭제’를 선택합니다.

<figure><img src="../../.gitbook/assets/image (427).png" alt=""><figcaption></figcaption></figure>



2. Warm Storage에서 고스트를 삭제한 폴더 또는 파일을 확인하고, 아이콘에서 배지가 제거된 것을 확인합니다.

<figure><img src="../../.gitbook/assets/image (428).png" alt=""><figcaption></figcaption></figure>
