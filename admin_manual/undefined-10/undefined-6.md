---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-10/undefined-6
---

# 사용자가 조작한 링크의 기록을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '로그 현황' > '링크 이력' 메뉴에서 사용자가 조작한 링크 기록을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* '로그 현황' > '링크 현황' 메뉴에는 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자의 설정 이력도 기록됩니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 이용할 수 있는 경우라도, Connect 폴더에서는 공유 링크를 생성할 수 없기 때문에 Connect 폴더의 링크 설정 정보는 확인할 수 없습니다.
* 링크를 생성한 이력은 '파일의 조작' 로그에 기록됩니다.\
  자세한 내용은 [사용자의 파일 이용 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/undefined-10/undefined-2)을 참조해 주십시오.
* 사용자 본인이 생성한 링크의 이력은 [사용자 페이지에서 Link History를 확인하는 방법](https://help.directcloud.net/user_manual/undefined-8/web-drive-link-history)에서 확인할 수 있습니다.
* 링크의 설정 정보는 '로그 현황' > '링크 현황'에서 확인 및 삭제할 수 있습니다.\
  자세한 내용은 [사용자가 생성한 링크의 설정 정보를 확인하는 방법](https://help.directcloud.net/admin_manual/undefined-10/undefined-4)을 참조해 주십시오.
* 계약 담당 관리자 또는 일반 관리자에 의해 삭제된 사용자는 '삭제된 사용자'로 표시됩니다.
* '링크 이력' 메뉴에서는 링크를 삭제할 수 없습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**링크 이력 확인**
{% endhint %}

1. '로그 현황' > '링크 이력' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1510).png" alt=""><figcaption></figcaption></figure>



2. '링크 이력'에서 링크 기록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (1511).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="184">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일/폴더명</td><td>링크가 생성된 파일 이름 또는 폴더 이름이 표시됩니다.</td></tr><tr><td>링크 URL</td><td>링크 URL이 표시됩니다.<br>"."는 "https://link.directcloud.net" 로 대체됩니다.</td></tr><tr><td>사용자</td><td>링크를 조작한 사용자의 이름이 표시됩니다.</td></tr><tr><td>날짜</td><td>링크가 조작된 날짜와 시간이 표시됩니다.</td></tr><tr><td>이벤트</td><td><p>링크에 관한 조작 내용이 표시됩니다.<br>조작의 종류는 다음과 같습니다.</p><ul><li>생성:<br>링크 생성</li><li>수정:<br>링크 수</li><li>알림메일 발송:<br>링크 이메일 보내기</li><li>업로드:<br>발신자가 링크 수신 화면에 파일 업로드</li><li>URL 변경:<br>링크 URL 변경</li><li>삭제:<br>링크 삭제</li></ul></td></tr><tr><td>내역</td><td>버튼을 클릭하면, 링크의 설정 정보 및 링크에 대한 접근 로그를 확인할 수 있는 '링크 이력 상세' 화면이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**링크 설정 정보 및 접근 내역 확인**
{% endhint %}

1. 링크의 설정 방법 및 접근 이력을 확인하려는 링크 이력의 '내역' 열에 있는 버튼을 클릭합니다.\
   링크 이력 세부사항 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1513).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. 링크 정보를 확인합니다.

<figure><img src="../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="193.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>링크 URL</td><td>링크 URL, 폴더 이름, 파일 이름이 표시됩니다.</td></tr><tr><td>이벤트(일시)</td><td>링크와 관련된 조작 내용과 조작된 날짜와 시간이 표시됩니다.</td></tr><tr><td>링크옵션</td><td>링크의 옵션 설정이 표시됩니다.<br>자세한 내용은 <a href="https://help.directcloud.net/user_manual/undefined-4/web">링크 생성 화면을 표시하여 기본 기능을 확인하는 방법</a>을 참조하십시오.</td></tr><tr><td>메일 내용</td><td>링크로 메일을 발송한 경우에는, 수신자 및 본문 등의 설정 내용이 표시됩니다.</td></tr><tr><td>읽기 내역</td><td><p>파일에 접근한 일시, IP 주소, 조작 내역이 표시됩니다.<br>자세한 내용은 아래와 같습니다.</p><ul><li>이메일 주소:<br><a href="https://help.directcloud.net/user_manual/undefined-4/web-drive">링크를 생성해 공유하는 방법</a>에서 '수신자 확인'에 체크한 경우에는 메일 주소가 표시됩니다.</li><li>날짜:<br>링크에 대한 접근 날짜 및 시간을 표시합니다.</li><li>IP 주소:<br>접속 원본의 IP 주소가 표시됩니다.</li><li>조작 내역:<br>링크 수신 화면에서 조작을 했을 경우 '미리 보기', '다운로드', '업로드'중 하나가 표시됩니다.</li></ul></td></tr></tbody></table>



{% hint style="warning" %}
**링크 이력을 필터링하여 표시**
{% endhint %}

링크 이력 화면에서 링크 기록을 기간, 조작, 사용자, 파일 이름, 링크 URL, 표시건수로 필터링할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>링크 이력을 표시할 기간을 '최근 7일', '최근 15일', '최근 1개월', '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작부터 현재까지 링크 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>클릭하여 드롭다운 목록을 보고 링크 이력을 필터링하여 보려는 작업을 선택합니다.</td></tr><tr><td>❹</td><td><p>클릭하여 드롭다운 리스트를 표시하고, 아래 중 하나의 검색 대상을 선택합니다. 기본값으로는 '전체'가 선택되어 있어, 모든 항목이 검색 대상이 됩니다.</p><ul><li>사용자명</li><li>사용자 ID</li><li>파일·폴더명</li><li>링크 URL</li></ul><p><strong>NOTE</strong>：<br>검색 대상을 선택하더라도 ❺의 키워드를 입력하지 않은 경우에는, 모든 항목이 검색 대상이 됩니다.<br>폴더명 검색은 링크가 생성된 파일이 저장되어 있는 폴더가 대상이 됩니다.<br>폴더 경로에 포함된 상위 폴더를 대상으로 검색할 수는 없습니다.</p></td></tr><tr><td>❺</td><td><p>❹에서 선택한 검색 대상의 키워드를 입력합니다.<br>링크 이력을 조작한 사용자, 파일·폴더명, 링크 URL로 필터링하려면, '사용자명' 또는 '사용자 ID', '파일·폴더명', '링크 URL'을 입력합니다.<br>링크 URL을 제외한 항목은 부분 일치로 검색되므로, 입력한 키워드가 포함된 검색 대상이 검색 결과에 표시됩니다.</p><p></p><p><strong>NOTE</strong>：<br>링크 URL은 완전 일치로 검색됩니다.<br>앞부분의 './'를 포함하지 않고 검색해 주십시오.</p></td></tr><tr><td>❻</td><td>링크 이력을 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**링크 이력을 CSV 파일로 다운로드**
{% endhint %}

1. 링크 이력에서 'CSV 다운로드' 버튼을 클릭합니다.\
   링크 이력은 대량의 데이터가 될 수 있으므로 미리 필터링하여 표시한 후 내보내는 것이 좋습니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1516).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1517).png" alt=""><figcaption></figcaption></figure>
