---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/folder_management/1st_folder
---

# 사용자 페이지에서 첫 번째 계층 구조의 폴더를 생성하는 방법

### 개요 <a href="#a03" id="a03"></a>

관리자로부터 "Shared Box"의 첫 번째 계층 폴더를 만들 수 있는 권한이 부여된 사용자는 "Shared Box" 바로 아래에 폴더를 만들 수 있습니다.\
이 매뉴얼에서는 사용자 페이지에서 "Shared Box"에 첫 번째 계층(1계층) 구조의 폴더를 생성하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 1계층 폴더를 생성하는 사용자는 폴더에 대한 접근 권한을 사용자에게 부여하는 방법 및 사용자에게 1계층 폴더 생성 권한을 부여하는 방법의 절차에 따라 1계층 폴더 생성 권한이 부여되어 있어야 합니다.
* 1계층 폴더 생성 권한을 가진 사용자는 접근 권한 종류나 Web 브라우저에서 가능한 작업과 상관없이 사용자 페이지에서 1계층 폴더를 생성할 수 있습니다.
* 1계층 폴더를 생성한 사용자는 자동으로 해당 폴더의 마스터가 됩니다.
* 1계층 폴더에 대해 마스터가 수행할 수 있는 작업은 폴더 이름 변경과 폴더 삭제만 가능합니다.
* <마스터> 권한이 없는 사용자는 1계층 폴더에 대한 작업을 수행할 수 없습니다.
* LDAP 연동 및 SAML 연동으로 등록된 사용자도 1계층 폴더 생성 권한이 부여되어 있는 경우에는 1계층 폴더를 생성할 수 있습니다.
* Guest에게 1계층 폴더 생성 권한을 부여할 수 없습니다.\
  따라서 Guest는 1계층 폴더를 생성할 수 없습니다.
* Guest에게 마스터 권한을 부여할 수 없습니다.\
  따라서 Guest는 1계층 폴더에 대한 작업을 수행할 수 없습니다.
* 폴더 이름은 190자 이내로 입력할 수 있습니다.
* 폴더 이름에 사용할 수 있는 문자와 사용할 수 없는 문자는 다음과 같습니다.
  * 사용할 수 있는 문자\
    UTF-8의 한자, 히라가나, 영문 대소문자, 숫자, 공백, 다국어 문자, 기호 및 이모지 등
  * 사용할 수 없는 문자\
    \ / : \* ? “ < > |
* 생성하는 폴더 이름에 구자체 문자가 포함된 경우 일부 문자는 자동으로 신자체로 변환될 수 있습니다.
* 폴더명 끝에 반각 마침표(.) 또는 공백 문자가 포함된 경우 Windows의 제한으로 인해 DirectCloud 드라이브에서는 해당 폴더를 사용할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Shared Box에 첫 번째 계층의 폴더 만들기**
{% endhint %}

1. Shared Box를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1255).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나를 사용하여 새 폴더 화면을 표시합니다.

&#x20;   ❶'새 폴더'버튼을 클릭

<figure><img src="../../.gitbook/assets/image (1256).png" alt=""><figcaption></figcaption></figure>

&#x20;     ❷ 슬라이드 화면에서 '새 폴더' 버튼을 클릭

<figure><img src="../../.gitbook/assets/image (1257).png" alt=""><figcaption></figcaption></figure>

&#x20;     새 폴더 화면이 표시됩니다.



3. 폴더 이름을 입력하고 권한을 부여할 대상 사용자를 선택한 다음 만들기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2336).png" alt="" width="375"><figcaption></figcaption></figure>

<table><thead><tr><th width="194.5">항목</th><th>설명</th></tr></thead><tbody><tr><td>모든 사용자</td><td>선택하면 지정한 사용자에게 접근 권한을 부여할 수 있습니다.</td></tr><tr><td>특정 사용자</td><td>선택하면 모든 사용자에게 전체권한 접근 권한이 부여됩니다.</td></tr></tbody></table>



4. 생성된 1계층 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1259).png" alt=""><figcaption></figcaption></figure>



5. 슬라이드 메뉴의 폴더 속성에 <마스터>로 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1260).png" alt=""><figcaption></figcaption></figure>
