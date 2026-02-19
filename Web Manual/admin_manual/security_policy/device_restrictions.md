---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/security_policy/device_restrictions
---

# 사용자가 이용할 수 있는 기기를 제한하는 방법

### 개요 <a href="#a03" id="a03"></a>

관리자가 승인한 기기에서만 DirectCloud를 사용할 수 있도록 하는 것을 기기인증이라고 합니다.\
기기 인증을 활성화하면, 관리 페이지에 등록되지 않은 기기에서 사용자가 로그인하려고 할 때 관리자의 승인이 필요하게 됩니다.\
이 매뉴얼에서는 '보안정책' > '접속 제어' 메뉴의 기기 관리 설정에서 디바이스 인증을 활성화하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 기기 관리는 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용됩니다.
* 사용자 > SSO 연동 메뉴에서 SAML2.0 연동의 사용함에 체크되어 있지 않은 경우에는 IdP 사용자를 포함한다 항목이 표시되지 않습니다.
* PC Web 브라우저 및 모바일 버전 Web 브라우저는 기기 관리 대상이 아닙니다.
* 기기 관리에서는 각 애플리케이션에서 아래 정보를 기반으로 접속한 기기를 판별합니다.
  * DirectCloud 드라이브: 볼륨 시리얼 번호와 사용자 ID
  * iOS: UUID
  * Android
    * 8.0 미만 버전: IMEI
    * Android 8.0 이상 버전: Android ID
* 특정 기기만 관리자의 승인을 거치도록 설정하는 것은 불가능합니다.
* 신규 기기의 처리를 모두 허가로 설정했더라도, 애플리케이션 이용 제한에서 해당 애플리케이션이 제한되어 있는 경우에는 로그인할 수 없습니다.
* 모두 허가에서 관리자의 승인이 필요로 설정을 변경한 경우, 이미 승인된 기기에 등록되어 있는 기기는 새로 승인의 대상이 되지 않으므로 승인 대기 기기 설정에 표시되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**기기 인증 설정**
{% endhint %}

1. '보안 정책' > '접속 제어' 메뉴를 선택하고 '기기 관리' 탭을 클릭하십시오.

<figure><img src="../../.gitbook/assets/image (592).png" alt=""><figcaption></figcaption></figure>



2. '신규 기기에서 로그인 시'의 '관리자의 허가 필요'를 선택합니다.

<figure><img src="../../.gitbook/assets/image (593).png" alt=""><figcaption></figcaption></figure>



3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (594).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**신규 기기 허용 또는 차단**
{% endhint %}

기기 인증 적용 대상 사용자가 로그인을 시도하면 계약 담당자와 일반 관리자에게 다음과 같은 "\[DirectCloud] ㅇㅇ님이 신규기기로 접속하였습니다." 라는메일이 발송됩니다.\
이 경우 다음 단계에 따라 기기를 허용하거나 차단합니다.

<figure><img src="../../.gitbook/assets/image (595).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

1. 보안 정책 > 접속 제어 메뉴를 선택하고 기기 관리 탭을 클릭하십시오.

<figure><img src="../../.gitbook/assets/image (596).png" alt=""><figcaption></figcaption></figure>



2. 승인요청 기기 설정 목록에서 허가가 또는 차단을 클릭합니다.\
   승인된 기기 메뉴에 장치 정보가 등록됩니다.

<figure><img src="../../.gitbook/assets/image (597).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. 승인된 기기 메뉴에서 승인자가 승인 또는 차단한 기기의 정보를 확인합니다.

<figure><img src="../../.gitbook/assets/image (598).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="210.800048828125">항목</th><th>설명</th></tr></thead><tbody><tr><td>사용자</td><td>승인된 기기를 사용하여 로그인한 사용자의 사용자 이름과 사용자 ID가 표시됩니다.</td></tr><tr><td>접속 기기</td><td><p>사용자가 로그인에 사용한 기기의 정보가 표시됩니다.<br>사용한 기기에 따라 표시되는 정보가 달라집니다.</p><ul><li>PC Agent, DirectCloud 드라이브:<br>컴퓨터 이름, OS 이름</li><li>iOS 애플리케이션:<br>기종 이름, OS 이름</li><li>Android 애플리케이션:<br>기종 모델명, OS 이름</li></ul><p></p><p><strong>NOTE</strong></p><ul><li>모바일 환경(iOS 애플리케이션, Android 애플리케이션)을 사용한 경우 모바일 아이콘이 표시됩니다.</li><li>iPhone과 iPad는 표시되는 OS 이름이 서로 다릅니다.<br>iPhone: iOS<br>iPad: iPadOS</li><li>iOS 기기를 사용하는 경우 설정 > 일반 > 정보를 열면 기종 이름을 확인할 수 있습니다.</li><li>Android 기기를 사용하는 경우 설정 > 기기 정보 등에서 기종의 모델명을 확인할 수 있습니다. 사용 중인 Android 기기에 따라 항목명이 다를 수 있습니다.<br>Android의 경우 일반적인 모델명(상품명, 시리즈명)이 아니라 기종의 모델명이 표시된다는 점에 유의해 주세요.</li></ul></td></tr><tr><td>최초 접속 정보</td><td>사용자가 승인된 기기에서 처음 로그인할 때 날짜와 시간과 IP 주소가 표시됩니다.</td></tr><tr><td>최종 접속 정보</td><td>사용자가 승인된 기기에서 마지막으로 로그인한 날짜와 시간과 IP 주소가 표시됩니다.</td></tr><tr><td>상태</td><td>기기의 승인 상태를 확인할 수 있습니다.</td></tr></tbody></table>



4. '허가' 또는 '차단' 후 상태를 전환하려면 '상태'항목에서 변경할 상태를 선택합니다.

<figure><img src="../../.gitbook/assets/image (599).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="147">항목</th><th>설명</th></tr></thead><tbody><tr><td>허가</td><td>상태가 '차단'인 장치를 '허가'으로 전환합니다.</td></tr><tr><td>차단</td><td>상태가 '허용'인 장치를 '차단'으로 전환합니다.</td></tr><tr><td>삭제</td><td>승인된 기기 목록에서 기기를 삭제합니다.<br>삭제하면 관리 페이지에서 상태를 전환할 수 없으며 계약 담당자 또는 일반 관리자가 다시 승인해야 합니다.</td></tr></tbody></table>
