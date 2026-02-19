---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/file_share/link_identification
---

# 공유 링크 생성 화면에서 공유 링크 수신자의 본인 확인을 강제하도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 ‘링크 옵션 설정’에서 링크 수신자가 수신 화면에 접근할 때 이메일 주소를 통한 본인 확인이 반드시 이루어지도록 하기 위해, 공유 링크 생성 화면에서 수신자의 ‘수신자 인증 의무사용'이 ‘사용함’으로 고정되도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* ‘링크 옵션 설정’은 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용되지만, Connect User에는 적용되지 않습니다.
* ‘수신자 인증 의무사용'를 ‘사용함’으로 설정한 경우, ‘링크 전송 방법’의 ‘링크 복사’와 ‘외부 메일러’는 선택할 수 없도록 비활성화됩니다.
* 2단계 인증을 사용하여 본인 확인을 수행하는 기능은 제공되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

**\[관리자 페이지에서의 설정]**

1. '보안 정책' > '반출 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1655).png" alt=""><figcaption></figcaption></figure>



2. 링크생성 시 기본값 설정의 수신자 인증 의무사용을 사용함으로 선택합니다.

<figure><img src="../../.gitbook/assets/image (1692).png" alt=""><figcaption></figcaption></figure>



3. 링크 옵션 설정에서 저장 버튼을 클릭합니다.



**\[사용자 페이지에서 설정]**

1. 공유 링크 만들기 화면에서 '이메일 옵션'을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1693).png" alt=""><figcaption></figcaption></figure>



2. '수신자 인증'의 '링크 접속 시 수신자 메일주소 입력'에 체크가 들어간 상태로 고정되어 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1694).png" alt=""><figcaption></figcaption></figure>
