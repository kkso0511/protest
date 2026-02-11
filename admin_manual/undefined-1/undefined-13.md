---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-1/undefined-13
---

# 공유 링크 생성 화면에서 외부 메일러로의 복사를 사용하지 못하도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 ‘링크 옵션 설정’에서 링크 생성 화면의 링크 공유 방법으로 ‘외부 메일러’를 사용하지 못하도록 제한하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* ‘링크 옵션 설정’은 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용되지만, Connect User에는 적용되지 않습니다.
* 워크플로우에서 '링크'의 '신청자'로 설정된 사용자의 경우 공유 링크 생성 화면에 '로컬 메일 발송' 아이콘이 표시되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

**\[관리자 페이지에서의 설정]**

1. '보안 정책' > '반출 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1654).png" alt=""><figcaption></figcaption></figure>



2. '링크생성 시 기본값 설정'의 '링크 발송방법 제어'에서 '로컬메일 발송 버튼 표시'를 선택 해제합니다.

<figure><img src="../../.gitbook/assets/image (1685).png" alt=""><figcaption></figcaption></figure>



3. 링크 옵션 설정에서 저장 버튼을 클릭합니다.



**\[사용자 페이지에서 설정]**

1. 공유 링크 생성 화면에서 '로컬메일 발송 버튼' 아이콘이 표시되지 않는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1688).png" alt=""><figcaption></figcaption></figure>
