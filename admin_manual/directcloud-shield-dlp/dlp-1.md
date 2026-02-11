---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/dlp-1
---

# 'DLP 설정'에서 사용자가 파일을 다운로드 할 수 있도록 설정하는 방법

### 개요

DLP(Data Loss Prevention) 기능을 사용하면 사용자가 파일을 조작하거나 외부로 반출하는 행위를 제한할 수 있습니다. DLP 폴더에 기밀 정보가 포함된 파일을 저장하면 의도치 않은 파일 유출을 방지할 수 있습니다.이 매뉴얼 에서는 'SHIELD' > 'DLP 설정' 메뉴에서 Web 브라우저 및 DirectCloud 드라이브의 DLP 폴더에 저장된 파일을 다운로드할 수 있도록 허용하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* 다운로드 설정은 기본으로 사용으로 설정되어 있습니다.
*   다운로드 작업을 수행하려는 사용자에게는 아래의 접근 권한이 부여되어 있어야 합니다.\
    <마스터>, <전체권한>, <편집자>, <다운로더>

    자세한 내용은 [접근 권한의 종류와 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/undefined) 항목을 참조하시기 바랍니다.
* '워크플로우' > '설정' 메뉴의 워크플로우 기본 설정에서 DLP 다운로드 워크플로우가 활성화되어 있는 경우에만 다운로드 설정이 가능합니다.
* DLP 설정 메뉴는 DirectCloud의 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에 표시됩니다.
* DirectCloud-SHIELD DLP는 다른 유료 옵션인 DirectCloud-SHIELD IRM으로 전환할 수 있습니다. \
  자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.

### 절차

{% hint style="info" %}
**다운로드 설정하기**
{% endhint %}

1. 'SHIELD' > 'DLP 설정' 메뉴를 선택하고 '파일 반출 정책' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

2. 다운로드 설정에서 '사용'을 선택하고 저장합니다.\
   \
   **NOTE:** 다운로드 워크플로우가 활성화 되어 있어야만 합니다.

<figure><img src="../../.gitbook/assets/image (168).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**다운로드가 허용되지 않은 경우의 애플리케이션 메뉴 표시**
{% endhint %}

DLP 설정에서 다운로드 설정이 사용하지 않음으로 설정된 경우, DLP 폴더에서는 파일을 다운로드할 수 없습니다.



**Web 브라우저**

Web 브라우저에서는 조작

&#x20;버튼이나 메뉴에 다운로드가 표시되지 않도록 변경됩니다.

* 조작 버튼

<figure><img src="../../.gitbook/assets/image (169).png" alt=""><figcaption></figcaption></figure>

* 마우스 오른쪽 클릭 메뉴

<figure><img src="../../.gitbook/assets/image (170).png" alt=""><figcaption></figcaption></figure>

* 파일 오른쪽 ▼ 버튼 메뉴

<figure><img src="../../.gitbook/assets/image (171).png" alt=""><figcaption></figcaption></figure>



**DirectCloud 드라이브**

* 워크플로우를 사용하도록 설정되어 있는 경우

마우스 오른쪽 버튼을 클릭했을 때 표시되는 메뉴에 다운로드가 표시됩니다.\
다운로드를 선택하면 워크플로우 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (173).png" alt=""><figcaption></figcaption></figure>

DLP 폴더에서 PC로 파일을 드래그 앤 드롭하여 다운로드하려고 시도하면, 화면 오른쪽 아래에 먼저 ‘보안 모드가 동작중입니다.’라는 메시지가 표시됩니다.\
그 후 ‘DLP 외부로 파일을 저장할 수 없습니다.’라는 오류가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (174).png" alt=""><figcaption></figcaption></figure>

* 워크플로우를 사용하지 않는 설정인 경우

마우스 오른쪽 버튼을 클릭했을 때 표시되는 메뉴에 다운로드가 표시되지 않게 됩니다.

<figure><img src="../../.gitbook/assets/image (175).png" alt="" width="563"><figcaption></figcaption></figure>

DLP 폴더에서 PC로 파일을 드래그 앤 드롭하여 다운로드하려고 시도하면, 화면 오른쪽 아래에 먼저 ‘보안 모드가 동작중입니다.’라는 메시지가 표시됩니다.\
그 후 ‘DLP 외부로 파일을 저장할 수 없습니다.’라는 오류가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (174).png" alt=""><figcaption></figcaption></figure>
