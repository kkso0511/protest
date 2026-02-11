---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/images-and-media/guest-2
---

# 사용자와 Guest에게 동시 로그인을 허용하지 않는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 로그인 설정 메뉴의 동시 로그인 제한 설정에서 애플리케이션 종류와 관계없이 사용자 및 Guest의 동시 로그인을 허용하지 않는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 동시 로그인 제한은 Guest에게도 적용되지만, Connect User, LDAP 연동으로 등록된 사용자에게는 적용되지 않습니다.
* SSO 로그인에도 동시 로그인 제한 설정이 적용됩니다. 이 경우 IdP에서 SAML 응답을 받은 뒤 로그인하는 애플리케이션이 제한 대상이 됩니다.
* 새롭게 로그인하면 기존 세션은 자동으로 로그아웃됩니다.
* DCMigrator도 DirectCloud 애플리케이션으로 동작하기 때문에, 이 매뉴얼의 절차로 동시 로그인을 금지하도록 설정한 경우, DCMigrator로 데이터 이전을 수행 중인 사용자와 동일한 사용자 ID로 다른 애플리케이션에 로그인하면 DCMigrator의 연결이 끊어지게 됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '보안 정책' > '로그인 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (744).png" alt=""><figcaption></figcaption></figure>



2. '동시 접속을 허가하지 않음'을 선택하고 '저장' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (752).png" alt=""><figcaption></figcaption></figure>
