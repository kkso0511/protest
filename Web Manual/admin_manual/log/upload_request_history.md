---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/log/upload_request_history
---

# 업로드 요청 이력과 업로드된 파일의 이력을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '로그 현황' > '업로드 요청 내역' 메뉴에서, 사용자가 업로드 요청에 대한 링크를 메일로 발송하여 파일 업로드를 요청한 이력을 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* 업로드 요청에는 폴더를 업로드할 수 없기 때문에, '업로드 요청' 화면에서 확인할 수 있는 것은 파일 업로드 이력만 해당됩니다.
* '로그 현황' > '업로드 요청 내역' 메뉴에는 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자의 업로드 요청 이력도 기록됩니다.
* Warm Storage, Cold Storage, 'DirectCloud-CONNECT'를 사용할 수 있는 환경이라 하더라도, Warm Storage, Cold Storage, Connect 폴더에서는 업로드 요청을 생성할 수 없기 때문에, '로그 현황' > '업로드 요청 내역' 메뉴에는 이력이 기록되지 않습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**업로드 요청 내역 확인**
{% endhint %}

1. '로그 현황' > '업로드 요청 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>



2. '업로드 요청 내역' 에서 업로드 요청 기록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="133.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>이름</td><td>업로드 요청의 링크를 발송한 사용자의 이름이 표시됩니다.</td></tr><tr><td>아이디</td><td>업로드 요청의 링크를 발송한 사용자의 ID가 표시됩니다.</td></tr><tr><td>업로드 요청</td><td>업로드 요청 설정 화면에서 입력한 제목과 업로드 요청의 경로가 표시됩니다.</td></tr><tr><td>날짜</td><td>업로드 요청의 링크를 발송한 일시가 표시됩니다.</td></tr><tr><td>받는 사람</td><td>업로드 요청의 링크를 발송한 메일의 발송 대상이 표시됩니다.</td></tr><tr><td>업로드 수</td><td>업로드 요청에 업로드된 파일의 수가 표시됩니다.</td></tr><tr><td>상태</td><td><p>업로드 요청의 상태가 표시됩니다.<br>자세한 내용은 아래와 같습니다.</p><ul><li>유효：<br>업로드 요청의 URL에 접근할 수 있는 상태</li><li>무효：<br>업로드 요청의 유효기간이 만료되어 URL에 접근할 수 없는 상태</li><li>삭제：<br>작성자 또는 계약 담당 관리자·일반 관리자에 의해 업로드 요청의 링크가 삭제되어 URL에 접근할 수 없는 상태</li></ul></td></tr><tr><td>동작</td><td>버튼을 클릭하면, 업로드 요청의 설정 정보 및 업로드 정보를 확인할 수 있는 화면이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**업로드 요청의 설정 정보 및 업로드 이력을 확인하기**
{% endhint %}

1. '업로드 요청'에서 업로드 요청의 설정 정보 및 업로드 이력을 확인하려는 업로드 요청 이력의 '동작' 열에 있는 버튼을 클릭합니다. '업로드 요청' 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

&#x20;   &#x20;

2. 설정 정보와 업로드 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>업로드 요청의 설정 정보가 표시됩니다.<br>자세한 내용은 <a href="https://help.directcloud.net/user_manual/file_share/wd_file_request">계정이 없는 상대로부터 파일을 받는 방법(업로드 요청 기능)</a>의 '절차'를 참조해 주십시오.</td></tr><tr><td>❷</td><td><p>업로드 요청에 파일이 업로드된 이력이 표시됩니다.<br>자세한 내용은 아래와 같습니다.</p><ul><li>업로드한 사용자의 메일 주소</li><li>업로드 일시</li><li>접속 원본의 IP 주소</li><li>업로드 화면에서 입력한 메시지</li><li>업로드한 파일의 이름 및 용량</li></ul></td></tr></tbody></table>



3. 업로드 요청의 설정 정보와 업로드 이력을 CSV 파일로 다운로드하려면, 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

4. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**업로드 요청 내역을 필터링하여 표시**
{% endhint %}

'업로드 요청' 화면에서는 업로드 요청의 이력을 기간, 사용자, 상태, 표시건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>업로드 요청 이력을 표시할 기간을, '최근 7일' '최근 15일' '최근 1개월' '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작일부터 현재까지의 업로드 요청 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>업로드 요청 이력을 필터링하여 표시할 상태로, '전체' '유효' '무효' '삭제' 중 하나를 선택합니다.</td></tr><tr><td>❹</td><td>업로드 요청 이력을 조작한 사용자로 필터링하려는 경우, '사용자명' 또는 '사용자 ID'를 입력합니다.</td></tr><tr><td>❺</td><td>업로드 요청 이력을 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**업로드 요청 내역을 CSV 파일로 다운로드**
{% endhint %}

1. '업로드 요청 내역'에서 'CSV 다운로드' 버튼을 클릭합니다. CSV 파일이 다운로드됩니다.\
   업로드 요청 내역은 대량의 데이터가 될 가능성이 있으므로, 미리 필터링하여 표시하고 나서 다운로드하는 것을 추천합니다.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
