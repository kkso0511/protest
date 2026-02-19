---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/log/two_factor_login_history
---

# 사용자가 2단계 인증을 통해 DirectCloud에 로그인한 기록을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '로그 현황' > '인증코드 발급 내역' 메뉴에서 사용자가 2단계 인증을 통해 DirectCloud에 로그인한 기록을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* '로그 현황' > '인증코드 발급 내역' 메뉴에는 Guest 및 LDAP 연동으로 등록된 사용자가 2단계 인증을 사용하여 로그인한 이력도 기록됩니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 이용할 수 있는 경우라도, Connect User에는 2단계 인증이 적용되지 않기 때문에, '인증코드 발급 내역' 메뉴에는 Connect User가 2단계 인증을 사용하여 로그인한 이력이 기록되지 않습니다.
* SAML 연동으로 등록된 사용자에게는 2단계 인증이 적용되지 않기 때문에, '인증코드 발급 내역' 메뉴에는 IdP 사용자가 2단계 인증을 사용하여 로그인한 이력이 기록되지 않습니다.
* 2단계 인증은 '이메일'을 통한 인증으로 진행됩니다.
* '인증코드 발급 내역' 메뉴에는 DirectCloud 이외의 서비스에 2단계 인증을 사용하여 로그인한 이력은 기록되지 않습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**2단계 인증 내역 확인**
{% endhint %}

1. '로그 현황' > '인증코드 발급 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1529).png" alt=""><figcaption></figcaption></figure>



2. 사용자가 2단계 인증 기능을 사용하여 DirectCloud에 로그인한 기록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (1530).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="161">항목</th><th>설명</th></tr></thead><tbody><tr><td>이름</td><td>로그인한 사용자의 이름이 표시됩니다.</td></tr><tr><td>아이디</td><td>로그인한 사용자의 ID가 표시됩니다.</td></tr><tr><td>이메일(전화번호)</td><td>인증코드가 전송된 이메일 주소 또는 전화번호가 표시됩니다.</td></tr><tr><td>발급요청시간</td><td>인증코드가 발행된 날짜와 시간이 표시됩니다.</td></tr><tr><td>접속 기기</td><td><p>로그인에 사용한 장치의 정보가 표시됩니다.<br>로그인에 사용한 응용 프로그램에 따라 표시되는 정보가 다릅니다.</p><ul><li>Web 브라우저:<br>Web Browser(PC)</li><li>PC Agent, DirectCloud 드라이브:<br>컴퓨터 이름(OS 이름)</li><li>iOS 애플리케이션, Android 애플리케이션:<br>모바일 기기의 제품명(OS명)</li></ul></td></tr><tr><td>용도</td><td><p>인증코드를 사용하여 로그인한 서비스 이름이 표시됩니다.</p><ul><li>2단계 인증(DirectCloud)</li></ul></td></tr><tr><td>인증코드 입력시간</td><td>사용자가 인증코드를 사용해 로그인한 날짜와 시간이 표시됩니다.<br>발행된 인증코드를 사용하여 로그인하지 않은 경우에는 비워 둡니다.</td></tr></tbody></table>



{% hint style="warning" %}
**2단계 인증 내역을 필터링하여 표시**
{% endhint %}

'인증코드 발급 내역' 화면에서 2단계 인증에 의한 로그인 기록을 기간, 사용자, 이메일 주소, 로그인 결과, 표시건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1531).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>2단계 인증으로 로그인한 이력을 표시할 기간을, '최근 7일' '최근 15일' '최근 1개월' '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작일부터 현재까지의 2단계 인증으로 로그인한 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td><p>2단계 인증으로 로그인한 이력을 로그인 결과로 필터링하려는 경우, 아래 중 하나를 선택합니다.</p><ul><li>인증코드 사용</li><li>인증코드 미사용</li></ul></td></tr><tr><td>❹</td><td>2단계 인증으로 로그인한 이력을 로그인한 사용자로 필터링하려는 경우, '사용자명' '사용자 ID' '메일 주소' 중 하나를 입력합니다.</td></tr><tr><td>❺</td><td>2단계 인증으로 로그인한 이력을 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**2단계 인증 내역을 CSV 파일로 다운로드하기**
{% endhint %}

1. '인증코드 발급 내역' 설정에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.\
   필요한 경우 인증코드 발급 내역을 필터링하여 다운로드하는 것이 좋습니다.

<figure><img src="../../.gitbook/assets/image (1532).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1533).png" alt=""><figcaption></figcaption></figure>
