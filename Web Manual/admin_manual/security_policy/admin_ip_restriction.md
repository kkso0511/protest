---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/security_policy/admin_ip_restriction
---

# 관리자 페이지에 로그인할 수 있는 IP 주소를 제한하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '보안 정책' > '접속 제어' 메뉴의 'IP 제한' 탭에서 관리자 페이지에 대한 액세스를 지정된 글로벌 IP 주소로 제한하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 상태가 '허가'로 설정된 경우, 등록된 글로벌 IP 주소를 모두 삭제하면 저장할 때 오류가 발생합니다.
* 잘못된 글로벌 IP 주소를 허가로 설정한 상태에서 로그아웃하면 관리 페이지에 접근할 수 없게 되므로 주의해 주세요.
* 등록 가능한 글로벌 IP 주소의 개수는 무제한입니다.
* 기본적으로 관리 페이지에 접속 중인 글로벌 IP 주소가 변경되면 세션이 끊어지므로 다시 로그인해야 합니다.\
  이 매뉴얼의 절차로 관리 페이지의 IP 주소 제한을 설정한 경우에도, 설정한 IP 주소 범위 내에서 글로벌 IP 주소가 변경되면 세션이 끊어집니다.
* 관리 페이지의 IP 주소 제한을 설정한 뒤에도 사용함 체크를 해제하면 설정 내용은 유지됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**관리 페이지의 IP 주소 제한 사용**
{% endhint %}

1. '보안 정책' > '접속 제어' 메뉴를 선택하고 'IP 제한' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (609).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 '관리자페이지 IP 제한' 설정을 표시하고 '사용'을 선택합니다.\
   설정은 즉시 저장됩니다.

<figure><img src="../../.gitbook/assets/image (610).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**지정된 글로벌 IP 주소에서만 액세스 허용**
{% endhint %}

1. 라디오 버튼의 '허가'를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2252).png" alt=""><figcaption></figcaption></figure>



2. 접근을 허용할 IP 주소 범위를 입력하고 추가 버튼을 클릭합니다.\
   입력한 IP 주소가 추가 됩니다.

{% hint style="info" %}
**NOTE**\
저장 시 접속이 차단되지 않도록 하려면 현재의 IP 주소에 표시된 글로벌 IP 주소가 포함되도록 설정해야 합니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2254).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

3. 필요에 따라 2단계를 반복하여 다른 IP 주소 범위를 추가합니다.



4. 저장 버튼을 클릭합니다.



5. 확인 화면에서 확인 버튼을 클릭합니다.\
   입력된 IP 주소로부터의 액세스만 허용되도록 설정됩니다.

<figure><img src="../../.gitbook/assets/image (613).png" alt=""><figcaption></figcaption></figure>





{% hint style="warning" %}
**지정된 글로벌 IP 주소에서 액세스를 차단.**
{% endhint %}

1. 라디오 버튼에서 '차단'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2255).png" alt=""><figcaption></figcaption></figure>



2. 접근을 차단할 IP 주소 범위를 입력하고 추가 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2256).png" alt=""><figcaption></figcaption></figure>



3. 필요에 따라 2단계를 반복하여 다른 IP 주소 범위를 추가합니다.



4. 저장 버튼을 클릭합니다.



5. 확인 화면에서 확인 버튼을 클릭합니다.\
   입력한 IP 주소에서의 접근이 차단되도록 설정됩니다.

<figure><img src="../../.gitbook/assets/image (613).png" alt=""><figcaption></figcaption></figure>
