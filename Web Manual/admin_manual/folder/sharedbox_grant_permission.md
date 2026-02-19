---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/folder/sharedbox_grant_permission
---

# Shared Box에 대한 접근 권한을 사용자에게 부여하는 방법

### 개요 <a href="#a03" id="a03"></a>

사용자, 그룹, Guest는 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission) 권한의 범위 내에서 폴더와 파일을 사용할 수 있습니다.\
이 매뉴얼에서는 폴더에 대한 접근 권한 및 접근 레벨을 사용자, 그룹, Guest, Connect User에게 부여하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '공유 설정' 메뉴를 사용할 수 있습니다.
* 이 매뉴얼에서는 Shared Box 폴더에서의 작업 방법을 설명하고 있지만, 다른 폴더에서도 동일한 절차로 작업할 수 있습니다.
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
**Shared Box의 사용자에게 접근 권한 부여**
{% endhint %}

**\[Shared Box 설정 화면 표시]**

1. '공유 설정' > 'Shared Box 관리' 메뉴를 선택하고 접근 권한을 설정하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1891).png" alt=""><figcaption></figcaption></figure>



**\[그룹, 사용자에게 권한설정]**

1. Shared Box 설정 화면의 구성원 관리에서 그룹/사용자의 오른쪽에 표시되는 '권한관리' 버튼을 클릭합니다.\
   권한 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1892).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. 그룹 또는 사용자를 선택합니다.&#x20;

<figure><img src="../../.gitbook/assets/image (1893).png" alt=""><figcaption></figcaption></figure>



3. 그룹을 선택한 경우 권한을 부여할 그룹을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1894).png" alt=""><figcaption></figcaption></figure>



4. 부여할 권한을 선택하고 추가 버튼을 클릭합니다.\
   선택한 그룹이 오른쪽 영역으로 이동합니다.

<figure><img src="../../.gitbook/assets/image (1895).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

5. '사용자'를 선택한 경우 권한을 부여하려는 사용자를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1896).png" alt=""><figcaption></figcaption></figure>

&#x20;  이때 사용자를 그룹으로 필터링하거나 사용자의 이름이나 ID로 필터링 검색할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1897).png" alt=""><figcaption></figcaption></figure>



6. 부여할 권한을 선택하고 추가 버튼을 클릭합니다.\
   선택한 사용자가 오른쪽 영역으로 이동합니다.

<figure><img src="../../.gitbook/assets/image (1898).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

7. 확인 버튼을 클릭합니다.\
   폴더 접근권한이 설정되고 Shared Box 메뉴로 돌아갑니다.

<figure><img src="../../.gitbook/assets/image (1899).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

8. 사용자 관리 설정의 '그룹/사용자' 아이콘에 추가한 그룹 사용자 수가 추가되었는지 확인하십시오.

<figure><img src="../../.gitbook/assets/image (1900).png" alt=""><figcaption></figcaption></figure>

<br>

**\[Guest에게 접근 권한 부여]**

1. Shared Box 설정 화면의 구성원 관리 설정에서 Guest 오른쪽에 표시되는 '권한관리' 버튼을 클릭합니다.\
   Guest의 권한 관리 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1901).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. 권한을 부여할 Guest를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1902).png" alt=""><figcaption></figcaption></figure>

&#x20;     이때 Guest의 이름이나 ID로 좁혀 검색할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1903).png" alt=""><figcaption></figcaption></figure>



3. 부여할 권한을 선택하고 추가 버튼을 클릭합니다.\
   선택한 Guest가 오른쪽 영역으로 이동합니다.

<figure><img src="../../.gitbook/assets/image (1904).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

4. 확인 버튼을 클릭합니다. \
   폴더 접근 권한이 설정되고 Shared Box 메뉴로 돌아갑니다.

<figure><img src="../../.gitbook/assets/image (1905).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

5. 사용자 관리 설정의 Guest 아이콘에 추가한 Guest 수가 더해져 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1906).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Connect User에게 접근 권한 및 접근 레벨을 부여**
{% endhint %}

1. '공유 설정' > 'Connect 관리' 메뉴를 선택하고, Connect User의 접근 권한 및 접근 레벨을 설정할 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>



2. '구성원 관리' 설정에서 'Connect User' 오른쪽에 표시된 '권한관리' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>



3. 권한을 부여할 Connect User를 선택합니다.

<figure><img src="../../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

이때 Connect User의 이름 또는 ID로 필터링 검색할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (48).png" alt="" width="545"><figcaption></figcaption></figure>



4. 부여하려는 접근 레벨을 선택하고 '추가' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>



5. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>



6. 구성원 관리 설정의 Connect User 아이콘에 추가한 Connect User 수가 더해져 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure>
