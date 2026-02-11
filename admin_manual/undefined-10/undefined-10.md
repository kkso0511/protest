---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-10/undefined-10
---

# 사용자가 파일첨부 메일을 발송한 이력을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '로그 현황'> '파일첨부 메일발송 내역' 메뉴에서 사용자가 첨부 파일을 보낸 내역을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* 폴더는 첨부 파일로 발송할 수 없습니다.\
  따라서 '파일첨부 메일발송' 메뉴에서 확인할 수 있는 것은 파일의 첨부 파일 발송 이력만 해당됩니다.
* '파일첨부 메일발송' 메뉴에는 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자의 첨부 파일 발송 이력도 기록됩니다.
* [사용자 페이지에서 파일첨부 메일발송의 이용 내역을 확인하는 방법](https://help.directcloud.net/user_manual/undefined-8/undefined-1)을 통해서도, 첨부 파일 발송 이력을 확인할 수 있습니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 이용할 수 있는 경우라도, Connect 폴더에서는 첨부 파일 발송을 이용할 수 없기 때문에, '로그 현황' > '파일첨부 메일발송 내역' 메뉴에는 Connect 폴더의 로그가 기록되지 않습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**파일첨부 메일발송 내역 확인**
{% endhint %}

1. '로그 현황'> '파일첨부 메일발송 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1534).png" alt=""><figcaption></figcaption></figure>



2. '파일첨부 메일발송 내역'에서 발송내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (1535).png" alt=""><figcaption></figcaption></figure>

| 항목    | 설명                                                                                                                                                                                                    |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 이름    | 첨부 파일을 발송한 사용자의 이름이 표시됩니다.                                                                                                                                                                            |
| 아이디   | 첨부 파일을 발송한 사용자의 ID가 표시됩니다.                                                                                                                                                                            |
| 제목    | <p>첨부 파일 발송 메일의 제목이 표시됩니다.<br>클릭하면 '상세' 화면에 첨부 파일 발송 메일의 상세 정보가 표시됩니다.<br>자세한 내용은 <a href="https://help.directcloud.net/user_manual/undefined-4/undefined-2">파일을 이메일에 첨부하여 전송하는 방법</a>을 참조해 주십시오.</p> |
| 받는 사람 | 첨부 파일 발송 메일의 발송 대상이 표시됩니다.                                                                                                                                                                            |
| 전송파일  | ZIP 형식으로 압축된 파일의 이름이 표시됩니다.                                                                                                                                                                           |
| 날짜    | 첨부 파일이 발송된 일시가 표시됩니다.                                                                                                                                                                                 |



{% hint style="warning" %}
**파일첨부 메일발송 내역을 필터링하여 표시**
{% endhint %}

'파일첨부 메일발송 내역'에서는 첨부파일 전송 내역을 기간, 사용자, 이메일 주소, 파일 이름, 표시건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1536).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>파일첨부 메일발송 내역을 표시하는 기간을 '최근 7일', '최근 15일', '최근 1개월', '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작부터 현재까지 파일첨부 메일발송 내역을 표시하는 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>파일첨부 메일발송 내역을 필터링하는 경우, 메일을 보낸 사용자의 '사용자 이름', '사용자 ID', 받는사람의 '이메일 주소' 또는 ZIP 형식으로 압축된 첨부 파일의 '파일 이름' 중 하나 를 입력합니다.</td></tr><tr><td>❹</td><td>첨부파일 전송 내역을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**파일첨부 메일발송 내역을 CSV 파일로 다운로드하기**
{% endhint %}

1. '파일첨부 메일발송 내역' 설정에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.\
   필요한 경우 파일첨부 메일발송 내역을 필터링하여 다운로드  하는 것이 좋습니다.

<figure><img src="../../.gitbook/assets/image (1537).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1538).png" alt=""><figcaption></figcaption></figure>
