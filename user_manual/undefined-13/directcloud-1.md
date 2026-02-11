---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-13/directcloud-1
---

# DirectCloud 드라이브 프록시 설정 방법

### 개요 <a href="#a03" id="a03"></a>

프록시 서버의 주소와 포트, 그리고 필요한 경우 프록시 서버의 인증 정보를 설정하면 프록시 서버를 통해 DirectCloud Drive에 접속할 수 있습니다.\
이 매뉴얼에서는 DirectCloud Drive에서 프록시 설정을 하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 Windows용 DirectCloud Drive를 예시로 설명합니다.
* 로그아웃 상태에서도 작업 메뉴의 DirectCloud 아이콘을 클릭하고 프록시 설정을 선택하면 프록시 설정 화면을 표시할 수 있습니다.
* 프록시 설정에서 지원하는 인증 방식은 Basic 인증만 해당되며, Kerberos 인증이나 NTLM 인증은 지원하지 않습니다.
* 프록시 설정에서 시스템의 프록시 설정 사용 또는 수동 프록시 설정을 선택한 경우, 다른 설정으로 전환하더라도 설정 정보는 유지됩니다.
* 시스템의 프록시 설정을 사용하는 경우에는 미리 'Windows의 설정' > '네트워크 및 인터넷' > '프록시에서 자동 프록시 설정 또는 수동 프록시 설정'을 구성해 두어야 합니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**프록시 설정 화면 표시**
{% endhint %}

1. DirectCloud 드라이브에 로그인합니다.<br>
2. 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (768).png" alt=""><figcaption></figcaption></figure>



3. 설정 화면의 오른쪽 상단에 있는 ⁝ 버튼을 클릭하고 표시된 메뉴에서 프록시 설정을 선택합니다.

<figure><img src="../../.gitbook/assets/image (769).png" alt=""><figcaption></figcaption></figure>

프록시 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (775).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**시스템의 프록시 설정 사용**
{% endhint %}

Windows에 설정된 프록시 설정을 사용하는 경우 다음 설정을 수행합니다.

1. 프록시 설정 화면에서 '시스템 설정을 이용' 을 선택합니다.\
   Windows에 설정된 프록시 서버의 주소와 포트 번호가 자동으로 반영됩니다.

<figure><img src="../../.gitbook/assets/image (771).png" alt=""><figcaption></figcaption></figure>



2. 프록시 서버 사용에 인증이 필요한 경우 '프록시 인증을 사용'을 선택하고 사용자 ID와 암호를 입력합니다.

<figure><img src="../../.gitbook/assets/image (773).png" alt=""><figcaption></figcaption></figure>



3. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (774).png" alt=""><figcaption></figcaption></figure>

설정이 저장되고 DirectCloud 드라이브가 다시 시작됩니다.



{% hint style="warning" %}
**수동으로 프록시 설정 입력**
{% endhint %}

수동으로 프록시 설정을 입력하는 경우 다음 설정을 수행합니다.

1. 프록시 설정 화면에서 '수동 설정을 이용'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (776).png" alt=""><figcaption></figcaption></figure>



2. 프록시 주소에 프록시 서버의 IP 주소 또는 URL을 입력하고 포트에 포트 번호를 입력합니다.

<figure><img src="../../.gitbook/assets/image (777).png" alt=""><figcaption></figcaption></figure>



3. 프록시 서버 사용에 인증이 필요한 경우 프록시 인증 사용을 선택하고 사용자 ID와 암호를 입력합니다.

<figure><img src="../../.gitbook/assets/image (778).png" alt=""><figcaption></figcaption></figure>



4. 확인 버튼을 클릭합니다.\
   설정이 저장되고 DirectCloud 드라이브가 다시 시작됩니다.

<figure><img src="../../.gitbook/assets/image (779).png" alt=""><figcaption></figcaption></figure>
