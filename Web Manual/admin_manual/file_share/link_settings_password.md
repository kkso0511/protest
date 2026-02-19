---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/file_share/link_settings_password
---

# 공유 링크 생성 화면에서 비밀번호 설정을 활성화/비활성화하는 방법

### 개요 <a href="#a03" id="a03"></a>

공유 링크의 비밀번호를 관리자가 강제로 설정하지 않고, 사용자 페이지의 공유 링크 생성 화면에서 설정할 수 있도록 하는 것도 가능합니다.\
이 매뉴얼에서는 ‘링크 옵션 설정’에서 공유 링크의 비밀번호를 사용자 측에서 변경할 수 있도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* ‘링크 옵션 설정’은 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용되지만, Connect User에는 적용되지 않습니다.
* 비밀번호 설정이 ‘사용’으로 고정되어 있는 경우에도, 사용자는 비밀번호 문자열을 자유롭게 변경할 수 있습니다.
* ‘비밀번호 정의’의 설정 내용은 공유 링크에는 적용되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**비밀번호 비활성화**
{% endhint %}

**\[관리자 페이지에서의 설정]**

1. '보안 정책' > '반출 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>



2. 링크생성 시 기본값 설정의 '비밀번호'를 '사용 안함'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>



3. 링크 옵션 설정에서 저장 버튼을 클릭합니다.



**\[사용자 페이지에서 작업]**

1. 관리자 페이지에서 기본값을 '사용안함'으로 설정한 경우, 사용자링크 생성 화면에서 비밀번호는 기본적으로 비활성화 되어 있습니다.

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>



2. 체크박스를 클릭해 활성화 할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**비밀번호 활성화**
{% endhint %}

**\[관리자 페이지에서 설정]**

1. '보안 정책' > '반출 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>



2. 링크생성 시 기본값 설정의 '비밀번호'를 '사용'으로 선택합니다.

<figure><img src="../../.gitbook/assets/image (100).png" alt=""><figcaption></figcaption></figure>



3. 링크 옵션 설정에서 저장 버튼을 클릭합니다.



**\[사용자 페이지에서 설정]**

1. 관리자 페이지에서 기본값을 '사용'으로 설정한 경우, 사용자링크 생성 화면에서 만료일은 기본적으로 활성화 되어 있습니다.

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>



2. 체크박스를 클릭해 비활성화 할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>
