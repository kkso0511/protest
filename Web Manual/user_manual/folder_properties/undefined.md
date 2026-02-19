---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/folder_properties/undefined
---

# 사용자 페이지의 특정 폴더에서 폴더 및 파일에 대한 링크 생성 기능을 활성화하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 메뉴얼에서는 사용자 페이지에서 Shared Box 폴더 또는 DLP폴더를 선택하고 "폴더 속성"에서 링크 만들기를 사용하도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 본 매뉴얼에서는 Shared Box와 DLP 폴더의 설정 방법을 설명하고 있습니다.
* 폴더 속성을 설정하는 사용자는 <마스터> 접근 권한이 부여되어 있어야 합니다.\
  자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission)을 참조해주시기 바랍니다.
* Shared Box의 폴더 속성에 있는 링크 항목은 첫 번째 계층의 폴더에서 설정할 수 있으며, 설정한 내용은 하위 폴더에도 그대로 적용됩니다.
* Shared Box의 폴더 속성의 링크 항목에는 관리 페이지의 [특정 폴더에서 링크 생성 기능을 활성화하는 방법](https://help.directcloud.net/admin_manual/folder/enable_link_creation)\
  의 내용이 반영됩니다.
* Shared Box에서는 [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)의 절차에서 워크플로우에 포함되지 않은 사용자의 기능을 제한하기를 선택한 경우, 신청자를 제외한 사용자와 Guest는 링크를 생성할 수 없습니다.
* Shared Box에서 [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)을 통해 워크플로우를 사용으로 설정하면, 폴더 속성에 워크플로우 메뉴가 표시됩니다.
* [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 DirectCloud-SHIELD IRM을 사용으로 설정하면 폴더 속성에 SHIELD 메뉴가 표시됩니다.\
  단, DLP 기능을 사용 중인 경우에는 이 메뉴가 표시되지 않습니다.
* [DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/admin_manual/directcloud-ai/enable_ai)에서 DirectCloud AI를 사용으로 설정하면 폴더 속성에 DirectCloud AI가 표시되며, 동시에 버전 관리 항목은 폴더 속성에서 사라집니다.
* DirectCloud-CONNECT를 이용할 수 있는 경우, 사용자 페이지에 Connect 메뉴가 표시됩니다.
* Connect 폴더의 폴더 속성에서는 워크플로우, SHIELD, 링크 설정을 할 수 없습니다.
* DirectCloud-SHIELD DLP를 이용 중인 경우, 사용자 페이지에 DLP 메뉴가 표시됩니다.
* 관리 페이지에서 DLP 폴더의 첫 번째 계층 폴더를 생성할 때는 링크 관련 설정이 표시되지 않으며, 링크 기능의 활성화 여부는 폴더 속성에서 설정해야 합니다.
* DLP 폴더에서 링크 관련 폴더 속성을 설정하려면, DLP 설정에서 사용자에게 링크 생성 권한을 허용하도록 설정 방법을 통해 링크 설정이 사용함으로 지정되어 있어야 합니다.\
  또한 관리자가 DLP의 워크플로우를 사용하지 않음으로 설정한 경우, 폴더 속성에 링크 설정은 표시되지 않습니다.
* DLP 폴더의 폴더 속성에는 본 문서에서 설명한 항목 외에도 아래 항목이 추가로 있습니다.
  * PDF 다운로드
  * 다운로드
  * 첨부 파일 전송
* DLP 폴더의 폴더 속성에서는 워크플로우, SHIELD, 링크 설정을 사용할 수 없습니다.
* DLP 폴더에서는 Connect User 초대를 사용할 수 없습니다.
* Warm Storage를 이용 중인 경우에는 사용자 페이지에 Warm Storage 메뉴가 표시됩니다.\
  Warm Storage에서는 링크 생성 기능을 사용할 수 없기 때문에, Warm Storage 폴더의 폴더 속성에는 링크 항목이 표시되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**폴더에서 링크 생성을 사용**
{% endhint %}

1. Shared Box 혹은 DLP 메뉴를 클릭한 뒤, 링크 설정을 활성화할 첫 번째 계층의 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1374).png" alt=""><figcaption></figcaption></figure>



2. 슬라이드 화면의 폴더 속성 설정에서 링크에 '사용함'이 표시되는지 확인합니다.\
   '사용 안함'이 표시되면 오른쪽에 표시된 설정 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1375).png" alt=""><figcaption></figcaption></figure>



3. '사용함'을 선택하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1376).png" alt=""><figcaption></figcaption></figure>
