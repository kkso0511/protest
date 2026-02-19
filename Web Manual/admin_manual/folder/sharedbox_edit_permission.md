---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/folder/sharedbox_edit_permission
---

# Shared Box에 대한 접근 권한을 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 사용자, 그룹, Guest 사용자에게 부여한 폴더에 대한 권한을 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '공유 설정' 메뉴를 사용할 수 있습니다.
* 이 글에서는 Shared Box 폴더에서의 작업 방법을 설명하고 있지만, 다른 폴더에서도 동일한 절차로 작업할 수 있습니다.
* 접근 권한은 폴더와 파일을 작업하기 위한 권한을 의미합니다.
* 접근 권한 레벨은 접근 권한이 부여된 폴더 안에 있는 폴더와 파일에 대해 가능한 작업을 정의한 것입니다.
* 접근 권한과 접근 권한 레벨은 최대 6단계까지 설정할 수 있습니다.
*   아래 화면에서는 각각 최대 3,000건까지 접근 권한을 표시할 수 있습니다.

    3,000건을 초과하면 확인 버튼을 눌 수 없게 되며, 자동으로 접근 권한 일괄 처리용 CSV 가져오기 화면이 표시됩니다.

    * 사용자의 접근 권한 설정 화면
    * Guest의 접근 권한 설정 화면
    * Connect User의 접근 권한 설정 화면
* 접근 권한 설정 버튼을 눌러도 반응이 없는 경우에는 web 브라우저의 캐시를 삭제한 후 다시 실행해주시기 바랍니다.
* DirectCloud-CONNECT를 사용할 수 있는 경우에는 Connect 관리 메뉴가 표시됩니다.
* DirectCloud-SHIELD DLP를 계약하고 있는 경우에는 DLP 관리 메뉴가 표시됩니다.
* Warm Storage를 사용할 수 있다면 Warm Storage 관리 메뉴가 표시됩니다.
* Cold Storage를 계약하고 있는 경우에는 Cold Storage 관리 메뉴가 표시됩니다.
* Cold Storage에서 접근 권한을 설정할 수 있는 폴더는 1단계 폴더만 해당되며, 설정 내용은 하위 폴더에 상속됩니다.
* Cold Storage에서는 다운로드와 미리보기를 사용할 수 없기 때문에 다운로더와 프리뷰어 접근 권한 레벨은 설정할 수 없습니다.
* Cold Storage 폴더에서 설정할 수 있는 접근 권한 수는 최대 100명까지이며, 단 <마스터>는 제외됩니다.
* Cold Storage에서는 접근 권한 설정 시 그룹을 선택할 수 없습니다.
* Cold Storage로 폴더를 이동하면 해당 폴더의 접근 권한 정보는 삭제됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Shared Box 폴더의 사용자 권한 변경**
{% endhint %}

**\[Shared Box 설정 화면 표시]**

1. '공유 설정' > 'Shared Box 관리' 메뉴를 선택하고 권한을 변경할 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1907).png" alt=""><figcaption></figcaption></figure>



**\[그룹/사용자의 권한 변경]**

1. Shared Box 설정 화면의 '구성원 관리' 설정에서 그룹/사용자의 오른쪽에 표시되는 '권한관리' 버튼을 클릭합니다. 그룹/사용자 권한관리 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1908).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. 권한을 변경하려는 그룹 또는 사용자의 드롭다운 목록에서 설정하려는 권한을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1909).png" alt=""><figcaption></figcaption></figure>



3. 확인 버튼을 클릭합니다. 설정한 권한이 저장됩니다.

<figure><img src="../../.gitbook/assets/image (1910).png" alt=""><figcaption></figcaption></figure>

&#x20;     <br>

**\[Guest의 권한 변경]**

1. Shared Box 설정 화면의 '구성원 관리' 설정에서 Guest의 오른쪽에 표시되는 '권한관리' 버튼을 클릭합니다.\
   Guest 권한관리 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1911).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. 권한을 변경하려는 Guest의 드롭다운 목록에서 권한을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1912).png" alt=""><figcaption></figcaption></figure>



3. 확인 버튼을 클릭합니다. 설정한 권한이 저장됩니다.

<figure><img src="../../.gitbook/assets/image (1913).png" alt=""><figcaption></figcaption></figure>
