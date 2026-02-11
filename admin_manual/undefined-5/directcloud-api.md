---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-5/directcloud-api
---

# DirectCloud API 키를 발급하는 방법

### 개요 <a href="#a03" id="a03"></a>

다른 시스템과 연동하여 기능과 데이터를 활용하기 위해 DirectCloud의 API를 사용할 수 있습니다.\
API를 사용하려면 API에서 액세스 토큰을 발행하는 방식에 따라 아래의 키를 발급받아야 합니다.

* 사용자·관리자별 API 키(Service 및 Service Key)를 발급받기
* 사용자 고유의 Access Key를 발행하기

이 매뉴얼에서는 관리자 페이지에서 위의 키를 발급받는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정' 항목에 접근 가능합니다.
* Web 브라우저에서 DirectCloud API를 호출할 수는 없습니다.
* DirectCloud API는 기본적으로 사용으로 설정되어 있으며, 사용자·관리자별 API 키(Service 및 Service Key)는 자동으로 발행됩니다.\
  Access Key는 기본적으로 사용 안함으로 설정되어 있습니다.
* 등록 가능한 Access Key의 수에는 제한이 없습니다.
* 1명의 사용자에게 여러 개의 Access Key를 발행할 수는 없습니다.
* 비활성 상태로 설정된 사용자의 Access Key로는 API를 사용할 수 없습니다.
* Access Key가 발행된 사용자가 삭제되면 사용자 항목에는 삭제된 사용자로 표시됩니다. 이 경우 Access Key는 무효가 되며 재발행하거나 복사할 수 없습니다.
* Access Key를 재발행하면 기존의 Access Key는 사용할 수 없게 됩니다.
* 사용자는 5자리에서 7자리의 user\_seq 코드로 관리되므로, 사용자 관련 작업을 수행할 때는 user\_seq 값을 지정해야 합니다.
* 그룹은 2자리의 group\_node로 관리되며, 그룹 생성 시에는 상위 그룹 코드 2자리와 새로 부여되는 그룹 코드 2자리가 조합되어 등록됩니다.\
  예를 들어 회사명 그룹의 그룹 코드가 AA인 경우, 그 하위에 첫 번째 그룹을 생성하면 AAAA가, 두 번째 그룹을 생성하면 AAAB가 등록됩니다.
* DirectCloud API로 그룹을 조작할 때는 group\_node가 아니라 group\_seq 값을 지정해야 합니다.
* 폴더는 노드 값이라는 고유한 값으로 관리되며, 이 값은 DirectCloud 관리자 API에서 폴더를 지정할 때 사용됩니다.
* Shared Box의 루트 폴더에는 1{2라는 값이 지정되어 있으며, 하위 폴더가 생성될 때마다 3자리씩 노드 값이 추가됩니다.\
  Shared Box를 조작할 때는 node 값을 지정해야 합니다.
* API로 Shared Box의 노드를 조작할 경우에는 관리 페이지에서 폴더 노드 값을 복사하는 방법을 이용해 가져오는 것을 권장합니다.
* My Box의 루트 폴더에는 1이라는 값이 지정되어 있으며, 하위 폴더가 생성될 때마다 3자리씩 노드 값이 추가됩니다.\
  다만 DirectCloud API로 My Box를 조작할 수는 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**API 키 얻기**
{% endhint %}

DirectCloud API에서 액세스 토큰 발행 및 Access Key를 사용한 액세스 토큰 발행 API를 실행할 때 필요한 API 키(Service 및 Service Key)를 발급받는 방법에 대해 설명합니다.

1.  '공유설정 '>  '맞춤형 설정' 메뉴를 선택합니다.<br>

    <figure><img src="../../.gitbook/assets/image (118).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 OpenAPI에서 OpenAPI 항목을 '사용'으로 설정합니다.

<figure><img src="../../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>



3. API Key 항목의'동작' 열의 '발급' 버튼을 눌러 Key를 발급 받습니다.

<figure><img src="../../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure>



4. API 키 설정에서 API를 실행하는 데 필요한 Service 및 Service Key를 참조합니다.

<figure><img src="../../.gitbook/assets/image (120).png" alt=""><figcaption></figcaption></figure>



4. Service Key를 복사하려면 사용자 또는 관리자의 Service Key 열에서 복사 버튼을 클릭합니다.\
   클립보드에 Service Key가 복사됩니다.

<figure><img src="../../.gitbook/assets/image (121).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

5. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (122).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Access Key 발급**
{% endhint %}

DirectCloud API에서 Access Key를 사용한 액세스 토큰 발행 API를 실행할 때 필요한 Access Key를 발행하는 방법에 대해 설명합니다.

1. '공유 설정' > '맞춤형 설정' 메뉴에서  OpenAPI 설정을 표시합니다.<br>
2. Access Key의 사용을 선택합니다.\
   Access Key 설정란이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure>



3. 추가 버튼을 클릭합니다. 사용자 추가 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (126).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

4. 사용자의 이름 또는 ID를 입력하고 검색 버튼을 클릭합니다. 사용자의 검색 결과가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (127).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

5. Access Key를 게시할 사용자의 '선택' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (128).png" alt=""><figcaption></figcaption></figure>



6. Access Key의 유효기간을 설정하려면 '무기한'을 선택 취소하고, 날짜 입력란을 클릭한 다음 달력에서 날짜를 클릭하거나 직접 날짜를 입력합니다.

<figure><img src="../../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure>



7. '발급' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (130).png" alt=""><figcaption></figcaption></figure>

Access Key가 발행됩니다.\
Access Key가 만료되면 '재발급' 버튼을 클릭하여 새 Access Key를 발행할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>



8. 액세스 키를 복사하려면 사용자의 Access Key 열에서 복사 버튼을 클릭합니다.\
   클립보드에 Access Key가 복사됩니다.

<figure><img src="../../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

9. '저장' 버튼을 클릭합니다.
