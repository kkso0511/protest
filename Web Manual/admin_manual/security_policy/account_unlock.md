---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/security_policy/account_unlock
---

# 계정 잠금을 수동으로 해제하는 방법

### 개요 <a href="#a03" id="a03"></a>

계정 잠금이 자동으로 해제되지 않도록 설정되어 있는 경우, 로그인에 연속으로 실패하여 잠긴 사용자의 계정을 수동으로 해제할 수 있습니다.\
이 매뉴얼에서는, 계정 잠금을 수동으로 해제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 계정 잠금 해제 절차는 어디에 로그인하는 과정에서 계정이 잠금되었는지에 따라 다릅니다.
  * **관리 페이지에 로그인할 때 계정이 잠금된 경우:**\
    계약 담당 관리자 또는 일반 관리자가 관리 페이지에 로그인하는 과정에서 계정이 잠금된 경우에는 '계정관리' > '관리자 추가'메뉴에서 계정 잠금을 해제합니다.
  * **애플리케이션에 로그인하는 과정에서 계정이 잠금된 경우:**\
    사용자, Guest, 그리고 계약 담당 관리자·일반 관리자가 아래 애플리케이션에 로그인할 때 계정이 잠금된 경우에는 '보안 정책' > '비밀번호 정책' 메뉴의 '차단자 현황' 탭에서 계정 잠금을 해제합니다.
    * PC 버전 Web 브라우저
    * PC Agent
    * DirectCloud 드라이브
    * iOS 애플리케이션
    * Android 애플리케이션
    * 모바일 버전 Web 브라우저
  *   애플리케이션에 로그인하는 과정에서 계정이 잠금된 사용자, Guest, 그리고 계약 담당 관리자·일반 관리자를 수동으로 해제하려면, 관리자 페이지에서 '보안정책' 항목에 접근 가능해야 합니다.

      또한 관리자 페이지의 '비밀번호 정책'->'정책 위반 설정'에서 '계정 차단 자동 복구' 기능이 허가안함 으로 되어있어야 합니다.
  *   관리 페이지에 로그인하는 과정에서 계정이 잠금된 계약 담당 관리자·일반 관리자를 수동으로 해제하려면, 관리자 페이지에서 '계정 관리' 항목에 접근 가능해야 합니다.

      또한 관리자 페이지의 '비밀번호 정책'->'정책 위반 설정'에서 로그인 실패 시 계정을 차단하는 기능이 선택되어 있어야 합니다.
  * 비밀번호 연속 오류로 인한 잠금은 Guest에게도 적용되지만, Connect User, LDAP 연동 및 SAML 연동으로 등록된 사용자에게는 적용되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**일반 관리자 · 계약 담당 관리자의 계정 잠금을 수동으로 해제**
{% endhint %}

1. '계정 관리' > '관리자 추가' 메뉴를 선택합니다.\
   계약 담당 관리자 또는 일반 관리자가 계정 잠긴 경우 '관리자 잠금' 열에 해제 버튼이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (741).png" alt=""><figcaption></figcaption></figure>



2. 계정 잠금을 해제하려는 사용자의 '해제' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (742).png" alt=""><figcaption></figcaption></figure>



3. 확인 버튼을 클릭하면 계정 잠금이 해제됩니다.

<figure><img src="../../.gitbook/assets/image (743).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자, Guest의 계정 잠금을 수동으로 해제**
{% endhint %}

1. '보안 정책' > '비밀번호 정책' 메뉴를 선택하고 '차단자 현황' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>



2. 계정 잠금을 해제하려는 계정의 '해제' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (739).png" alt=""><figcaption></figcaption></figure>



3. 확인 버튼을 클릭하면 계정 잠금이 해제됩니다.

<figure><img src="../../.gitbook/assets/image (740).png" alt=""><figcaption></figcaption></figure>
