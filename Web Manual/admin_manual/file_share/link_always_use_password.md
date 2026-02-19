---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/file_share/link_always_use_password
---

# 공유 링크 생성 화면에서 암호 설정을 항상 사용하도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 ‘링크 옵션 설정’에서 관리자가 설정한 공유 링크의 비밀번호를 사용자에게 강제로 적용하여 사용자 페이지에서 변경할 수 없도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* ‘링크 옵션 설정’은 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용되지만, Connect User에는 적용되지 않습니다.
* ‘비밀번호 정의’의 설정 내용은 공유 링크에는 적용되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

**\[관리자 페이지에서의 설정]**

1. '보안 정책' > '반출 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>



2. 링크생성 시 기본값 설정의 '비밀번호'에서 '항상 사용'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (101).png" alt=""><figcaption></figcaption></figure>



3. 링크 옵션 설정에서 저장 버튼을 클릭합니다.



**\[사용자 페이지에서 설정]**

1. 관리자 페이지에서 '항상 사용'으로 설정한 경우, 사용자 링크 생성 화면에서는 비밀번호를 비활성화할 수 없습니다.(체크박스 해제 불가능)

<figure><img src="../../.gitbook/assets/image (1674).png" alt=""><figcaption></figcaption></figure>
