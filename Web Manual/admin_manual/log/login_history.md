---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/log/login_history
---

# 사용자의 로그인 기록을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '로그 현황' > '로그인 내역'메뉴에서 사용자의 로그인 기록을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* Guest, LDAP 연동 및 SAML 연동으로 취득한 사용자의 로그인 이력도 기록됩니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 이용할 수 있는 경우라도, Connect User의 로그인 이력은 기록되지 않습니다.
* DirectCloud-SHIELD IRM 및 DC Migrator 에서 로그인한 이력도 기록됩니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**사용자의 로그인 내역 확인**
{% endhint %}

1. '로그 현황' > '로그인 내역'메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1489).png" alt=""><figcaption></figcaption></figure>



2. 로그인 설정에서 사용자의 로그인 기록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (1490).png" alt=""><figcaption></figcaption></figure>

| 항목     | 설명                                                                                                                                                                                                                                                                          |
| ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 이름     | 로그인한 사용자의 이름이 표시됩니다.                                                                                                                                                                                                                                                        |
| 아이디    | 로그인한 사용자의 ID가 표시됩니다.                                                                                                                                                                                                                                                        |
| 접속 기기  | <p>로그인할 때 사용한 장치 정보가 표시됩니다.<br>로그인한 각 응용 프로그램 유형마다 표시되는 정보가 다릅니다.</p><ul><li>Web 브라우저<br>&#x3C;PC>, OS 이름</li><li>PC Agent, DirectCloud 드라이브<br>컴퓨터 이름, OS 이름</li><li>iOS 애플리케이션, Android 애플리케이션<br>모바일 기기 제품 이름, OS 이름</li><li>모바일 web 브라우저<br>&#x3C;모바일>, OS 이름</li></ul> |
| 어플리케이션 | <p>로그인한 애플리케이션이 표시됩니다.<br>각 응용 프로그램 유형마다 표시되는 정보가 다릅니다.</p><ul><li>Web 브라우저<br>애플리케이션 정보, 브라우저 이름</li><li>PC Agent, DirectCloud 드라이브<br>애플리케이션 정보, 애플리케이션 버전</li><li>iOS 애플리케이션, Android 애플리케이션<br>애플리케이션 정보, OS 버전</li><li>DCMigrator<br>애플리케이션 정보, 애플리케이션 버전</li></ul>    |
| 접속 아이피 | <p>연결할 IP 주소와 <a href="https://help.directcloud.net/admin_manual/security_policy/user_ip_restriction">사용자 페이지에 로그인할 수 있는 IP 주소를 제한하는 방법</a>으로 허용된 IP 주소인지 여부에 따라 다음 정보 중 하나가 표시됩니다.</p><ul><li>허용된 IP 주소의 경우:<br>사내</li><li>허용되지 않는 IP 주소의 경우:<br>사외</li></ul>              |
| 날짜     | 사용자가 로그인한 날짜와 시간이 표시됩니다.                                                                                                                                                                                                                                                    |
| 서비스    | <p>사용자가 로그인한 서비스의 이름이 표시됩니다.</p><ul><li>표시되는 서비스 이름:<br>DirectCloud, DirectCloud-SHIELD</li></ul>                                                                                                                                                                           |
| 상태     | <p>사용자가 로그인하면 다음 중 하나가 표시됩니다.</p><ul><li>로그인 성공</li><li>로그인 실패</li><li>유효기간 만료</li><li>로그인 차단</li><li>web 접속 차단</li><li>자동 로그인</li><li>기기 차단</li><li>아이피 차단</li></ul>                                                                                                       |



{% hint style="warning" %}
**로그인 내역을 필터링하여 표시**
{% endhint %}

필터링설정을 사용하면 기간, 사용자, 로그인 결과, 건수별로 로그인 내역을 필터링할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1491).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="93.60003662109375">No.</th><th width="656">설명</th></tr></thead><tbody><tr><td>❶</td><td>로그인 내역을 표시할 기간을, '최근 7일', '최근 15일', '최근 1개월', '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작부터 현재까지의 로그인 내역을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td><p>로그인 내역을 로그인 결과로 필터링하려면 다음 로그인 결과 중 하나를 선택합니다.</p><ul><li>로그인 성공</li><li>로그인 실패</li><li>유효기간 만료</li><li>로그인 차단</li><li>web 접속 차단</li><li>자동 로그인</li><li>기기 차단</li><li>아이피 차단</li></ul></td></tr><tr><td>❹</td><td>로그인 내역을 로그인한 사용자로 필터링하려면, 사용자 이름 또는 사용자 ID를 입력합니다.</td></tr><tr><td>❺</td><td>로그인 내역을 표시할 건수를 「10」「25」「50」「100」 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**로그인 내역을 CSV 파일로 다운로드 하기**
{% endhint %}

1. 로그인 설정에서 'CSV 다운로드' 버튼을 클릭합니다.\
   로그인 이력은 대량의 데이터가 될 수 있으므로 미리 필터링하여 표시한 후 다운로드하는 것이 좋습니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1492).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1493).png" alt=""><figcaption></figcaption></figure>
