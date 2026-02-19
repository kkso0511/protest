---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/security_policy/login_one_device
---

# 사용자와 Guest에게 애플리케이션별로 하나의 로그인만 허용하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 로그인 설정 메뉴의 동시 로그인 제한 설정에서 사용자와 Guest에게 애플리케이션별로 하나의 로그인만 허용하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 동시 로그인 제한은 Guest에게도 적용되지만, Connect User, LDAP 연동으로 등록된 사용자에게는 적용되지 않습니다.
* SSO 로그인에도 동시 로그인 제한 설정이 적용됩니다. 이 경우 IdP에서 SAML 응답을 받은 뒤 로그인하는 애플리케이션이 제한 대상이 됩니다.
*   PC 버전 Web 브라우저, PC Agent, DirectCloud 드라이브, iOS 애플리케이션, Android 애플리케이션, 모바일 버전 Web 애플리케이션에서 로그인한 경우 각각의 로그인마다 하나의 연결이 유지됩니다.

    단, 이 매뉴얼의 절차로 설정하는 경우 PC 버전 Web 브라우저와 모바일 버전 Web 브라우저 각각에서 로그인에 사용할 수 있는 브라우저는 하나만 허용됩니다.
* 동시 로그인 제한은 기본적으로 동시 로그인을 금지하는 것으로 설정되어 있습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '보안 정책' > '로그인 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (745).png" alt=""><figcaption></figcaption></figure>



2. '각 어플리케이션별로 1개씩 접속 허가'를 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (751).png" alt=""><figcaption></figcaption></figure>
