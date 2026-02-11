---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/images-and-media/undefined-7
---

# 사용자가 로그인했을 때 알림 메일이 발송 되도록 관리 페이지에서 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

로그인 알림 설정에서 로그인 알림 메일을 활성화하면, 사용자 정보 관리에 등록된 사용자가 로그인할 때 해당 사용자의 이메일 주소로 로그인 알림 메일이 전송됩니다.\
이를 통해 제3자에 의한 부정 로그인(사칭)을 감지할 수 있습니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 로그인 알림 설정은 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용됩니다.
* 관리 페이지에서 로그인 알림을 활성화해도, 사용자 페이지에서 알림 메일 설정을 받지 않음으로 설정한 경우에는 알림 메일이 전송되지 않습니다.
* 사용자 페이지의 알림 메일 설정을 받음으로 설정했더라도, 관리 페이지의 로그인 알림이 비활성화되어 있는 경우에는 알림 메일이 전송되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '보안 정책' > '로그인 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 로그인 알림 설정을 표시한 다음, 알림 메일발송의 '사용'에 체크하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (755).png" alt=""><figcaption></figcaption></figure>

사용자가 로그인하면 로그인한 사용자의 이메일 주소로 다음과 같은 알림 이메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (756).png" alt=""><figcaption></figcaption></figure>
