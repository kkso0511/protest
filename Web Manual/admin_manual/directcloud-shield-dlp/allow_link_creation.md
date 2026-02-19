---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/allow_link_creation
---

# 'DLP 설정'에서 사용자에게 링크 생성을 허용하는 방법

### 개요

DLP(Data Loss Prevention) 기능을 사용하면 사용자가 파일을 조작하거나 외부로 반출하는 행위를 제한할 수 있습니다. DLP 폴더에 기밀 정보가 포함된 파일을 저장하면 의도치 않은 파일 유출을 방지할 수 있습니다.이 매뉴얼 에서는 'SHIELD' > 'DLP 설정' 메뉴에서 Web 브라우저 및 DirectCloud 드라이브의 DLP 폴더에 저장된 파일에 대해 링크 생성을 허용하도록 설정하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* 링크 설정은 기본으로 사용으로 설정되어 있습니다.
*   파일 링크 생성을 수행하려는 사용자에게는 아래의 접근 권한이 부여되어 있어야 합니다.

    * <마스터>, <전체권한>, <편집자>

    자세한 내용은 [접근 권한의 종류와 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission) 항목을 참조하시기 바랍니다.
* 폴더 링크 생성을 수행하려는 사용자에게는 아래의 접근 권한이 필요합니다.
  * <마스터>, <전체권한>
* 워크플로우 > 설정 메뉴의 워크플로우 기본 설정에서 DLP 링크 워크플로우가 활성화되어 있는 경우에만 링크 생성이 가능합니다.
* DLP 설정 메뉴는 DirectCloud의 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에 표시됩니다.
* DirectCloud-SHIELD DLP는 다른 유료 옵션인 DirectCloud-SHIELD IRM으로 전환할 수 있습니다. \
  자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.

### 절차

{% hint style="warning" %}
**DLP 설정에서 링크 생성을 허용하기**
{% endhint %}

1. 'SHIELD' > 'DLP 설정' 메뉴를 선택하고 '파일 반출 정책' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

2. 링크 설정에서 사용에 체크한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2450).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**링크 생성이 허용되지 않은 경우의 애플리케이션 메뉴 표시**
{% endhint %}

DLP 설정에서 다운로드 설정이 사용하지 않음으로 지정되어 있는 경우, DLP 폴더에서는 링크 생성이 불가능합니다.\
Web 브라우저 및 DirectCloud 드라이브에서는 조작버튼이나 메뉴에서 링크가 표시되지 않도록 변경됩니다.



**\[Web 브라우저]**

* 조작버튼

<figure><img src="../../.gitbook/assets/image (2451).png" alt=""><figcaption></figcaption></figure>

* 마우스 오른쪽 클릭 메뉴

<figure><img src="../../.gitbook/assets/image (2452).png" alt=""><figcaption></figcaption></figure>

* 파일 오른쪽 ▼ 버튼 메뉴

<figure><img src="../../.gitbook/assets/image (2453).png" alt=""><figcaption></figcaption></figure>



**\[DirectCloud 드라이브]**

마우스 오른쪽 버튼을 클릭했을 때 표시되는 메뉴에 '링크생성'이 표시되지 않습니다.

<figure><img src="../../.gitbook/assets/image (175).png" alt="" width="563"><figcaption></figcaption></figure>
