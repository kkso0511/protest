---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/workflow/request_list
---

# 워크플로우 신청 목록을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

워크플로우를 사용하면 사용자가 다음 작업을 수행할 때 결재자가 승인할 수 있도록 설정할 수 있습니다.

* 다운로드
* 링크전송
* 파일첨부 메일발송
* 업로드

워크플로우의 신청자로 지정된 사용자가 대상 기능을 이용하기 위한 승인 신청을 하고, 워크플로우의 결재자로 지정된 사용자에 의해 승인됨으로써, 비로소 조작이 가능해지는 구조입니다.\
이 매뉴얼에서는, '워크플로우' > '워크플로우 현황' 메뉴에서, 사전에 생성된 워크플로우 설정에 따라 신청된 승인 신청 목록과, 승인 신청의 상세 정보를 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '워크플로우' 항목을 사용할 수 있습니다.
* 워크플로우를 이용하려면 [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)의 절차에 따라, '워크플로우 설정'에서 '사용'이 선택되어 있어야 합니다.
* [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)에서 워크플로우가 활성화되어 있더라도, [특정 폴더에서 워크플로우를 활성화하 방법](https://help.directcloud.net/admin_manual/folder/enable_workflow)에서 '워크플로우' 설정이 '사용 안함'으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
* '다운로드' 워크플로우에서는, 한 번에 200개를 초과하는 파일의 다운로드를 신청할 수 없습니다.
* '업로드' 워크플로우에서는, 한 번에 100개를 초과하는 파일의 업로드를 신청할 수 없습니다.
* '업로드' 워크플로우에서 업로드할 수 있는 파일 용량의 합계는, 5GB까지입니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**워크플로우 현황 목록 보기**
{% endhint %}

1. '워크플로우' > '워크플로우 현황' 메뉴를 선택합니다.\
   '워크플로우 현황'화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2089).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. 사용자의 워크플로우 신청 목록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2090).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="161">항목</th><th>설명</th></tr></thead><tbody><tr><td>제목</td><td>사용자가 워크플로우를 신청할 때 입력한 '제목'이 표시됩니다.</td></tr><tr><td>기능</td><td><p>워크플로우의 대상이 되는 기능이 표시됩니다.<br>복수의 기능이 대상의 경우, '00(기능) 외 0건'이라고 표시됩니다.</p><ul><li>다운로드:<br>파일 다운로드</li><li>링크전송:<br>폴더 및 파일 링크 생성</li><li>파일첨부 메일발송:<br>파일첨부 메일 생성</li><li>업로드:<br>파일 업로드</li></ul></td></tr><tr><td>신청자</td><td>워크플로우를 신청한 사용자의 이름이 표시됩니다.</td></tr><tr><td>기안일</td><td>워크플로우가 신청된 날짜와 시간이 표시됩니다.</td></tr><tr><td>결재자</td><td>'상태'가 '승인' 또는 '거절'인 경우 워크플로우를 승인하고 거절한 결재자가 표시됩니다.</td></tr><tr><td>결재일</td><td>'상태'가 '승인' 또는 '거절'인 경우 워크플로우가 승인되고 거절된 날짜와 시간이 표시됩니다.</td></tr><tr><td>상태</td><td><p>워크플로우 신청의 상태로, 아래 중 하나가 표시됩니다.</p><ul><li>대기:<br>결재자, 대리 결재자가 신청을 열람하기 전 상태</li><li>열람 중:<br>참조자, 결재자, 대리 결재자가 신청을 열람한 상태</li><li>승인:<br>결재자, 대리 결재자가 신청을 승인한 상태</li><li>거절:<br>결재자, 대리 결재자가 신청을 반려한 상태</li><li>회수:<br>신청자가 신청을 철회한 상태</li><li>반송:<br>신청이 승인되기 전에 워크플로우가 삭제된 상태</li><li>삭제:<br>신청자가 '취소' 상태인 신청을 삭제한 상태</li></ul></td></tr><tr><td>동작</td><td><p>'상세' 버튼을 클릭하면, '상세' 화면에 아래 정보가 표시됩니다.</p><ul><li>워크플로우</li><li>결재자</li><li>상태</li></ul><p>또한 워크플로우의 신청 대상이 되는 '기능'에 따라, 워크플로우의 상세 정보가 표시됩니다.</p></td></tr></tbody></table>



{% hint style="warning" %}
**워크플로우 신청 목록을 필터링하여 표시**
{% endhint %}

'워크플로우 현황'에서는 사용자에 의해 신청된 워크플로우 신청 목록을 '기간, 상태, 기능, 제목, 신청자'등으로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="86.4000244140625">No.</th><th width="644.7999877929688">설명</th></tr></thead><tbody><tr><td>1</td><td>현재까지 신청된 워크플로우 신청을 표시할 기간을, '최근 7일', '최근 15일', '최근 1개월', '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>2</td><td>현재까지 신청된 워크플로우 신청을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은, 12개월입니다.</td></tr><tr><td>3</td><td>클릭하여 드롭다운 리스트를 표시하고, 워크플로우 신청 목록을 필터링하여 표시하고 싶은 상태를 선택한 뒤, 기능에 체크합니다.</td></tr><tr><td>4</td><td>워크플로우 신청 목록을 워크플로우의 제목이나 워크플로우를 생성한 사용자로 필터링하는 경우에는, '제목', '사용자명' 또는 '사용자 ID'를 입력합니다.</td></tr><tr><td>5</td><td>워크플로우 신청을 표시할 건수를, '10', '25', '50', '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**워크플로우 목록을 CSV 파일로 다운로드**
{% endhint %}

1. '워크플로우 현황' 목록에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (2092).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열어 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2093).png" alt=""><figcaption></figcaption></figure>
