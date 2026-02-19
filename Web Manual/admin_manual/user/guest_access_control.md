---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/guest_access_control
---

# Guest에게 접근 제어 설정을 적용할지 선택하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 'Guest' 관리 메뉴에서 '보안 정책' > '접근 제어'의 애플리케이션 이용 제한, IP 주소 제한 설정을 Guest에게도 적용할지 선택하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* [사용자가 이용할 수 있는 애플리케이션을 제한하는 방법](https://help.directcloud.net/admin_manual/security_policy/app_restrictions), [사용자 페이지에 로그인할 수 있는 IP 주소를 제한하는 방법](https://help.directcloud.net/admin_manual/security_policy/user_ip_restriction)의 절차로 사용자·Guest에게 적용된 설정 정보는, [특정 사용자·Guest에게 예외적인 접근 제한을 부여하는 방법](https://help.directcloud.net/admin_manual/security_policy/access_individual_settings)에서 설정한 내용으로 덮어쓰기됩니다.
* 또한 [특정 사용자·Guest에게 예외적인 접근 제한을 부여하는 방법](https://help.directcloud.net/admin_manual/security_policy/access_individual_settings)에서 적용된 설정 정보는 이 매뉴얼 의 절차로 설정한 정보로 다시 덮어쓰기됩니다.
* Guest 보안 설정에서는 기기 관리와 이중 인증 설정은 사용할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Guest 설정 보기**
{% endhint %}

1. '계정 관리' > 'Guest' 메뉴를 선택하여 Guest 설정 탭을 표시합니다.

<figure><img src="../../.gitbook/assets/image (1729).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 '보안 예외 설정'을 표시합니다.

<figure><img src="../../.gitbook/assets/image (1821).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Guest에 사용자와 동일한 애플리케이션 사용 제한을 적용할지 여부 설정**
{% endhint %}

1. '보안 예외 설정'에서 '웹 브라우저' 사용 설정을 지정한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1822).png" alt=""><figcaption></figcaption></figure>

| 항목             | 설명                                                                                       |
| -------------- | ---------------------------------------------------------------------------------------- |
| 보안 정책에 따름      | '접속 제어'>'접속 제어 개별설정' 메뉴에서 설정한 애플리케이션 이용 제한을 Guest에도 적용하려면 선택합니다.                         |
| Guest는 제약없이 사용 | '접속 제어'>'접속 제어 개별설정' 메뉴에서 설정한 응용 프로그램 사용 제한을 따르지 않고 web 브라우저프로그램을 사용할 수 있도록 허용하려면 선택합니다. |



{% hint style="warning" %}
**Guest에 사용자와 동일한 IP 주소 제한을 적용할지 여부 설정**
{% endhint %}

1. '보안 예외설정에'서 'IP 접속 제한'을 설정하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1823).png" alt=""><figcaption></figcaption></figure>

| 항목             | 설명                                                               |
| -------------- | ---------------------------------------------------------------- |
| 보안 정책에 따름      | '접속 제어'>'접속 제어 개별설정' 메뉴에서 설정한 IP 주소 제한을 Guest에도 적용하려면 선택합니다.     |
| Guest는 제약없이 사용 | '접속 제어'>'접속 제어 개별설정' 메뉴에서 설정한 IP 주소 제한을 따르지 않고 액세스를 허용하려면 선택합니다. |
