---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/allow_file_attach_email
---

# 'DLP 설정'에서 사용자에게 파일첨부 메일발송 기능을 허용하는 방법

### 개요

DLP(Data Loss Prevention) 기능을 사용하면 사용자가 파일을 조작하거나 외부로 반출하는 행위를 제한할 수 있습니다. DLP 폴더에 기밀 정보가 포함된 파일을 저장하면 의도치 않은 파일 유출을 방지할 수 있습니다.이 매뉴얼 에서는 'SHIELD' > 'DLP 설정' 메뉴에서 Web 브라우저의 DLP 폴더에 저장된 파일을 첨부해 메일발송  하는것을 허용하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* 파일첨부 메일발송 설정은 기본으로 '사용'으로 설정되어 있습니다.
*   파일첨부 메일발송을 수행하려는 사용자에게는 아래의 접근 권한이 부여되어 있어야 합니다.

    * <마스터>, <전체권한>, <편집자>

    자세한 내용은 [접근 권한의 종류와 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission) 항목을 참조하시기 바랍니다.
* 파일첨부 메일발송 기능은 Web 브라우저에서만 사용할 수 있습니다.
* 파일첨부 메일발송 시 파일은 ZIP 형식으로 압축되어 전송됩니다.
* 워크플로우 > 설정 메뉴의 워크플로우 기본 설정에서 DLP의 파일첨부 메일발송 워크플로우가 활성화된 경우에만 파일첨부 메일발송 설정이 가능합니다.
* DLP 설정 메뉴는 DirectCloud의 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에 표시됩니다.
* DirectCloud-SHIELD DLP는 다른 유료 옵션인 DirectCloud-SHIELD IRM으로 전환할 수 있습니다. \
  자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.

### 절차

{% hint style="warning" %}
**파일첨부 메일발송 설정하기**
{% endhint %}

1. 'SHIELD' > 'DLP 설정' 메뉴를 선택하고 '파일 반출 정책' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

2. 파일첨부 메일발송 설정에서 '사용'에 체크한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2454).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**파일첨부 메일발송이 허용되지 않은 경우의 애플리케이션 메뉴 표시**
{% endhint %}

DLP 설정에서 파일첨부 메일발송 설정이 사용하지 않음으로 지정된 경우, DLP 폴더에서는 파일을 첨부하여 전송할 수 없습니다.

Web 브라우저에서는 작업 버튼이나 메뉴에 파일첨부 메일발송이 표시되지 않도록 변경됩니다.



**\[Web 브라우저]**

* 조작버튼

<figure><img src="../../.gitbook/assets/image (2451).png" alt=""><figcaption></figcaption></figure>

* 마우스 오른쪽 클릭 메뉴

<figure><img src="../../.gitbook/assets/image (2452).png" alt=""><figcaption></figcaption></figure>

* 파일 오른쪽 ▼ 버튼 메뉴

<figure><img src="../../.gitbook/assets/image (2453).png" alt=""><figcaption></figcaption></figure>











