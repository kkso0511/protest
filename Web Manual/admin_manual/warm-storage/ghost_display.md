---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/warm-storage/ghost_display
---

# Warm Storage로 이동 한 폴더 및 파일의 고스트 표시 여부를 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 ‘Warm Storage’를 제공합니다.\
일반적인 Hot Storage에서 링크나 버전 관리 등 일부 기능을 제외한 Warm Storage는 더 저렴한 비용으로 이용할 수 있습니다.\
예를 들어, 자주 사용하지 않는 폴더 계층의 데이터를 모두 Warm Storage로 이동하여 장기 보관하면, Shared Box의 Storage를 효율적으로 활용할 수 있습니다.\
이 매뉴얼에서는 Warm Storage로 이동한 폴더와 파일의 고스트를 표시할지에 대한 여부를 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* Warm Storage를 사용할 수 있다면 Warm Storage 관리 메뉴가 표시됩니다. 또한 '공유 설정' > '세부 기능 설정' 메뉴에 고스트 표시 설정이 나타납니다.
*   Shared Box의 폴더와 파일이 Warm Storage로 이동되면, 이동 전 위치에 표시되는 정보를 고스트라고 부릅니다.\
    고스트는 흐린 색으로 표시되며, 아이콘 오른쪽 아래에 Warm Storage 배지가 함께 표시됩니다.

    * 사용자 페이지에서의 고스트 표시 예(폴더)\
      ![](<../../.gitbook/assets/image (421).png>)
    *   사용자 페이지에서의 고스트 표시 예(파일)

        <div align="left"><figure><img src="../../.gitbook/assets/image (420).png" alt="" width="207"><figcaption></figcaption></figure></div>

    고스트에는 이동된 위치, 이동 일시, 이동을 수행한 사용자와 같은 정보만 포함되어 있습니다. 폴더나 파일의 실제 데이터가 아니므로 클릭해도 해당 폴더로 이동하거나 파일을 표시할 수 없으며, 체크박스로 선택할 수도 없습니다.

    고스트를 삭제할 수는 있지만, 이를 삭제해도 이동된 실제 폴더나 파일이 삭제되는 것은 아닙니다.

    고스트를 활용해 폴더나 파일 정보를 확인하거나 원래 위치로 되돌리는 방법은 [사용자 페이지에서 고스트(Ghost)를 조작하는 방법](https://help.directcloud.net/user_manual/warm-storage/use_ghost)을 참고해주시기 바랍니다.
* 고스트 표시 설정은 기본적으로 '사용'으로 설정되어 있습니다.
* '고스트 표시 설정'을 '사용 안함'으로 설정하면, 이미 존재하는 고스트는 비표시됩니다.\
  단, Warm Storage로 이동된 폴더 및 파일에 추가된 배지는 비표시되지 않기 때문에, 이동 전의 정보를 확인할 수 있습니다.\
  Warm Storage로 이동된 폴더 및 파일의 정보를 확인하는 방법에 대해서는, [Warm Storage로 폴더 또는 파일을 이동하는 방법](https://help.directcloud.net/user_manual/warm-storage/wd_move_to_warm)을 참조해 주십시오.
* 고스트 표시 설정을 다시 '사용'으로 되돌리면, 숨겨졌던 고스트가 다시 화면에 표시됩니다.
* 고스트는 다른 폴더로 이동할 수 없습니다.
* 고스트는 폴더나 파일의 실제 데이터가 아니므로, 같은 폴더 안에 고스트와 동일한 이름의 폴더나 파일을 업로드하거나 이동하거나 복사할 수 있습니다. 다만 고스트에서 동일한 이름의 폴더나 파일을 원래대로 되돌릴 수는 없습니다.
* Warm Storage로 이동된 폴더나 파일의 이름이 변경되거나 위치가 이동되면, 그 내용이 고스트에도 반영됩니다.
* Warm Storage로 이동된 폴더나 파일이 삭제되면 고스트도 함께 삭제됩니다.
* Warm Storage로 이동된 폴더나 파일을 Warm Storage가 아닌 다음 위치로 이동한 경우, 고스트는 아래와 같이 처리됩니다.
  * 이동 원본이 아닌 Shared Box:\
    고스트는 삭제됩니다.
  * Shared Box가 아닌 다른 폴더:\
    고스트는 삭제되지 않으며, 고스트의 저장 위치 정보만 변경됩니다.
* 고스트는 사용자 휴지통이나 관리자 휴지통으로 이동되지 않으므로 삭제된 경우 복원할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '공유설정' > '세부 기능 설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2261).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 'Warm Stroage로 이동한 흔적 표시' 를 확인하고 설정 합니다.

<figure><img src="../../.gitbook/assets/image (2262).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="181.5">항목</th><th>설명</th></tr></thead><tbody><tr><td>자동이동 시 흔적 표시</td><td><p>파일이 자동으로 Warm Storage로 이동될 때 고스트를 표시할지 여부를 설정합니다.</p><ul><li>사용<br>고스트를 표시합니다.</li><li>사용 안함<br>고스트를 표시하지 않습니다.</li></ul></td></tr><tr><td>수동이동 시 흔적 표시</td><td><p>폴더와 파일을 수동으로 Warm Storage로 이동했을 때 고스트를 표시할지 여부를 설정합니다.</p><ul><li>사용<br>고스트를 표시합니다.</li><li>사용 안함<br>고스트를 표시하지 않습니다.</li></ul></td></tr></tbody></table>



3. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2263).png" alt=""><figcaption></figcaption></figure>
