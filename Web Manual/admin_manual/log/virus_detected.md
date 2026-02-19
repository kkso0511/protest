---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/log/virus_detected
---

# 바이러스가 감지된 파일을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

바이러스에 감염된 파일을 DirectCloud에 업로드하려고 하면, 알려진 바이러스의 패턴 매칭 또는 동작 감지(휴리스틱 감지)에 의해 감지된 파일은 자동으로 삭제됩니다.\
이 매뉴얼에서는, 바이러스에 감염된 파일의 업로드 이력을 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* 바이러스가 감지된 파일은, 즉시 삭제됩니다.
* 바이러스가 감지되면, 파일을 업로드한 사용자에게 메일로 알림이 전송됩니다.\
  관리자에게는 알림이 전송되지 않습니다.
* DirectCloud의 바이러스 검지는, 아래 방법을 지원합니다.
  * 패턴 매칭\
    알려진 바이러스의 패턴 파일과 비교하여 바이러스를 검지하는 방법
  * 동작 감지(휴리스틱 감지)\
    프로그램의 동작을 통해 바이러스를 검지하는 방법
* 아래에 해당하는 파일은, 바이러스 검지 대상에서 제외됩니다.
  * 500MB를 초과하는 압축 파일
  * 1GB를 초과하는 비압축 파일
* 바이러스의 최신 패턴 파일은 2시간마다 확인되어, 자동으로 최신 상태로 유지됩니다.\
  패턴 파일이 갱신되면, '로그' > '바이러스 검지' 메뉴의 '바이러스 및 위협 방지'의 '갱신 일시'가 업데이트됩니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**바이러스 검출 내역 확인**
{% endhint %}

1. '로그 현황' > '바이러스 검출 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1479).png" alt=""><figcaption></figcaption></figure>



2. 사용자가 바이러스에 감염된 파일을 업로드하면 아래와 같이 업로드 실패메시지가 표시되고 바이러스검출 내역에 상세 내용을 확인 할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1480).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1482).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="181">항목</th><th>설명</th></tr></thead><tbody><tr><td>이름</td><td>파일을 업로드한 사용자의 이름이 표시됩니다.</td></tr><tr><td>아이디</td><td>파일을 업로드한 사용자의 ID가 표시됩니다.</td></tr><tr><td>검출내역</td><td>감지된 바이러스의 이름이 표시됩니다.</td></tr><tr><td>파일</td><td>바이러스가 감지된 파일의 이름이 표시됩니다.</td></tr><tr><td>날짜</td><td>파일을 업로드한  날짜와 시간이 표시됩니다.</td></tr><tr><td>크기</td><td>업로드 시도한 파일의 용량이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**바이러스 검출 내역을 필터링 하여 표시**
{% endhint %}

필터링설정을 사용하면 기간, 사용자, 파일 이름, 건수별로 바이러스 검출 내역을 필터링할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1483).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="116">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>바이러스 탐지 내역을 표시하는 기간을 최근 7일, 최근 15일, 최근 1개월, 최근 3개월 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작부터 현재까지 바이러스 탐지 내역을 표시하는 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>바이러스 탐지 기록을 사용자 또는 파일 이름으로 필터링하려면 파일을 업로드한 사용자의 '사용자 이름', '사용자 ID' 또는 '파일 이름'을 입력합니다.</td></tr><tr><td>❹</td><td>바이러스 탐지 내역을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**바이러스 검출 내역을 CSV 파일로 다운로드 하기**
{% endhint %}

1. 바이러스 검출 내역에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1484).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1485).png" alt=""><figcaption></figcaption></figure>
