---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/dlp-4
---

# DLP 폴더에 저장된 폴더와 파일의 반출 이력을 확인하는 방법

### 개요

이 매뉴얼 에서는 DLP 폴더에 저장된 폴더 또는 파일을 반출한 이력을 확인하는 방법을 설명합니다.\
폴더 또는 파일을 반출할 수 있는 작업은 아래와 같습니다.

* 링크: 폴더 또는 파일 반출
* PDF 다운로드, 다운로드, 파일첨부 메일발송: 파일 반출

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* DLP 설정 메뉴는 DirectCloud의 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에 표시됩니다.
* DirectCloud-SHIELD DLP는 다른 유료 옵션인 DirectCloud-SHIELD IRM으로 전환할 수 있습니다. \
  자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* 사용자 작업 이력 확인 방법을 통해 DLP 폴더에서 폴더나 파일을 반출한 이력을 확인할 수도 있습니다.\
  다만 PDF 다운로드 작업 이력은 다운로드로 기록됩니다.
* 다운로드되는 CSV 파일의 문자 인코딩은 환경설정 > 상세 설정 메뉴의 다운로드 시 문자 코드 설정에서 지정할 수 있습니다.\
  자세한 내용은 [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참조하시기 바랍니다.

### 절차

{% hint style="info" %}
**폴더·파일 반출 이력을 확인하기**
{% endhint %}

1. 'SHIELD' > 'DLP 파일반출 내역' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2457).png" alt=""><figcaption></figcaption></figure>

2. DLP 파일반출 내역 설정에서 DLP 폴더에서 파일이 반출된 이력을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2458).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="172.39996337890625">항목</th><th>설명</th></tr></thead><tbody><tr><td>행위</td><td><p>폴더 또는 파일의 반출 작업으로 아래 항목 중 하나가 표시됩니다.</p><ul><li>PDF 다운로드</li><li>다운로드</li><li>링크</li><li>파일첨부 메일발송</li></ul></td></tr><tr><td>파일/폴더명</td><td><p>반출 작업 유형에 따라 반출된 폴더 또는 파일의 이름이 표시됩니다.</p><ul><li>PDF 다운로드, 다운로드, 파일첨부 메일발송의 경우:<br>파일 이름</li><li>링크의 경우:<br>파일 이름 또는 폴더 이름</li></ul><p>또한, 위의 파일 또는 폴더가 저장되어 있는 폴더 경로도 함께 표시됩니다.</p></td></tr><tr><td>이름</td><td>폴더 또는 파일을 반출한 사용자의 이름이 표시됩니다.</td></tr><tr><td>기기</td><td><p>아이콘에 마우스 커서를 올리면, 폴더 또는 파일을 반출한 기기의 정보를 확인할 수 있습니다. 사용한 애플리케이션에 따라 표시되는 정보가 달라집니다.</p><ul><li>웹 브라우저:  웹브라우저</li><li>DirectCloud 드라이브: 컴퓨터 이름</li></ul></td></tr><tr><td>접속 아이피</td><td><p>접속한 IP 주소가 표시됩니다.</p><p>또한 사용자 페이지에 로그인할 수 있는 IP 주소를 제한하는 방법에서 허용된 IP 주소인지 여부에 따라 아래 정보 중 하나가 표시됩니다.</p><ul><li>허용된 IP 주소인 경우: 사내</li><li>허용되지 않은 IP 주소인 경우: 사외</li></ul></td></tr><tr><td>날짜</td><td>폴더 또는 파일이 반출된 날짜와 시간이 표시됩니다.</td></tr><tr><td>크기</td><td>반출된 파일의 용량이 표시됩니다.<br>폴더의 경우 0B로 표시됩니다.</td></tr><tr><td>동작</td><td><p>표시된 버튼을 클릭하면 반출 작업 유형에 따라 아래 화면이 표시됩니다.</p><p>다운로드 작업의 경우에는 상세 화면이 존재하지 않으므로 확인 버튼이 표시되지 않습니다.</p><ul><li>PDF 다운로드:<br>PDF 문서 생성 내역</li><li>링크:<br>링크 이력</li><li>파일첨부 메일발송:<br>메일 세부 내용</li></ul></td></tr></tbody></table>



**PDF 문서 생성 내역 확인**

1. DLP 파일반출 내역 설정에서, 상세 내용을 확인하려는 PDF 다운로드 이력의 동작 열에 표시된 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2464).png" alt=""><figcaption></figcaption></figure>

2. PDF 문서 생성 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2460).png" alt="" width="562"><figcaption></figcaption></figure>

<table><thead><tr><th width="195.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일명</td><td>다운로드된 PDF 파일의 이름이 표시됩니다.</td></tr><tr><td>날짜</td><td>PDF 다운로드가 실행된 일시가 표시됩니다.</td></tr><tr><td>크기</td><td>다운로드된 PDF 파일의 용량이 표시됩니다.</td></tr></tbody></table>



**링크 이력 확인**

1. DLP 파일반출 내역 설정에서, 상세 내용을 확인하려는 '링크' 이력의 동작 열에 표시된 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2465).png" alt=""><figcaption></figcaption></figure>

2. 링크 이력을 확인합니다.\
   링크 이력의 상세 화면에 표시되는 각 항목에 대해서는, [사용자가 생성한 링크의 설정 정보를 확인하는 방법](https://help.directcloud.net/admin_manual/undefined-10/undefined-4)의 링크 설정 정보와 접근 이력을 확인하는 부분을 참고해주시기 바랍니다.

<figure><img src="../../.gitbook/assets/image (2462).png" alt="" width="563"><figcaption></figcaption></figure>



**파일첨부 메일발송 이력의 상세 내용을 확인합니다.**

1. DLP 파일반출 내역 설정에서, 상세 내용을 확인하려는 파일첨부 메일발송 이력의 동작 열에 표시된 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2466).png" alt=""><figcaption></figcaption></figure>

2. 파일첨부 메일발송 이력의 상세 내용을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2467).png" alt="" width="559"><figcaption></figcaption></figure>

<table><thead><tr><th width="155.5999755859375">항목</th><th>설명</th></tr></thead><tbody><tr><td>보낸 사람</td><td>파일을 메일로 전송한 사용자의 이름이 표시됩니다.</td></tr><tr><td>받는 사람</td><td>파일을 전송한 메일의 수신자 메일 주소가 표시됩니다.</td></tr><tr><td>제목</td><td>파일을 전송한 메일의 제목이 표시됩니다.</td></tr><tr><td>내용</td><td>파일을 전송한 메일의 본문이 표시됩니다.</td></tr><tr><td>첨부파일</td><td>첨부된 파일의 이름이 표시됩니다. 첨부 파일은 ZIP 형식으로 압축되므로 확장자는 .zip으로 표시됩니다.</td></tr><tr><td>비밀번호</td><td>첨부된 ZIP 파일을 해제할 때 필요한 비밀번호와 비밀번호 전달 방식이 표시됩니다.</td></tr></tbody></table>

{% hint style="info" %}
**폴더와 파일의 반출 이력을 필터링하여 표시하기**
{% endhint %}

DLP 폴더의 파일 반출 이력 화면에서는 폴더와 파일의 반출 이력을 기간, 항목, 사용자, 파일명, 건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2468).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="81.20001220703125">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>반출 이력을 표시할 기간을 직전 7일, 직전 15일, 직전 1개월, 직전 3개월 중에서 선택합니다.</td></tr><tr><td>2</td><td>계약 시작일부터 현재까지의 반출 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>3</td><td>클릭하여 드롭다운 리스트를 표시하고, 반출 이력을 필터링하여 표시할 작업에 체크합니다.</td></tr><tr><td>4</td><td>반출 이력을 작업을 수행한 사용자나 파일명으로 필터링하려는 경우, 사용자명 또는 사용자 ID, 파일명을 입력합니다.</td></tr><tr><td>5</td><td>반출 이력을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>

{% hint style="info" %}
**폴더와 파일의 반출 이력을 CSV 파일로 다운로드기**
{% endhint %}

1. DLP 파일반출 내역 설정에서 CSV 다운로드 버튼을 클릭합니다.\
   필요에 따라 폴더나 파일의 반출 이력을 먼저 필터링한 후 다운로드하는 것을 권장합니다.

<figure><img src="../../.gitbook/assets/image (2469).png" alt=""><figcaption></figcaption></figure>

2. CSV 파일을 열어 정상적으로 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2470).png" alt=""><figcaption></figcaption></figure>
