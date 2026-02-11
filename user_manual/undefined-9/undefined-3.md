---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-9/undefined-3
---

# 다운로드 워크플로우를 신청하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 워크플로우를 이용하면 사용자가 아래 작업을 수행할 때 결재자의 승인을 받도록 설정할 수 있습니다.

* 파일 다운로드
* 폴더 및 파일의 링크 생성
* 파일첨부 메일발송
* 파일 업로드

워크플로우 신청자로 지정된 사용자가 대상 기능을 사용하기 위해 승인 신청을 하고, 워크플로우 결재자로 지정된 사용자가 이를 승인함으로써 비로소 작업이 가능해지는 구조입니다.\
이 매뉴얼 에서는 Web 브라우저와 DirectCloud 드라이브에서 파일 다운로드 워크플로우를 신청하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리 페이지에서 '워크플로우'가 '사용' 으로 활성화되어 있더라도, '공유설정'->' Shared Box 관리' 에서\
  '워크플로우'가 사용안함’으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
* 한 번에 200개를 초과하는 파일 다운로드를 신청할 수 없습니다.
* 신청자로 등록된 Guest는 승인 신청, 내용 변경, 철회, 삭제를 할 수 있습니다.
*   다음 작업이 수행되면 대리 결재자 또는 결재자에게 알림 메일이 발송됩니다.\
    단, 신청 내용 변경이나 신청 삭제의 경우에는 알림 메일이 발송되지 않습니다.

    * 신청자에 의한 승인 신청
    * 신청자에 의한 신청한 워크플로우의 철회
    * 대리 결재자 또는 결재자에 의한 워크플로우의 승인 또는 거절

    신청자에게는 다음 작업이 수행될 때 알림 메일이 발송됩니다.

    * 대리 결재자 또는 결재자에 의한 워크플로우의 승인 또는 거절
* 대리 결재자 또는 결재자에 그룹이 등록되어 있는 경우,\
  승인 요청이 제출되면 그룹에 속한 모든 사용자의 이메일 주소로 승인 요청 알림 메일이 발송됩니다.
*   워크플로우 설정에서 ‘자동 결재’에 체크되어 있는 경우,  선택한 일수가 경과한 후 0시 0분에 자동으로 결재됩니다.\
    단, 설정한 날의 자정(0시 0분)까지를 하루로 계산합니다.

    예를 들어, 설정일이 2023년 8월 7일 13시이고 자동 승인을 1일로 설정한 경우, 그날 밤 2023년 8월 8일 0시 0분에 자동 결재됩니다.
*   ‘다운로드’, ‘업로드’ 워크플로우에서 신청자로 설정된 사용자는 DirectCloud Drive에서 다음 작업을 수행할 수 없습니다.

    * 드래그 앤 드롭을 통한 다운로드 및 업로드
    * 직접 편집
    * 이름 변경
    * 폴더 및 파일 이동
    * 폴더 및 파일 복사
    * 폴더 생성
    * 폴더 및 파일 삭제

    다음 작업은 가능합니다.

    * 마우스 오른쪽 버튼 메뉴를 통한 다운로드 및 업로드
    * 미리보기
    * 온라인 편집
    * 링크 생성
    * 버전 관리
    * 파일 잠금

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 다운로드 승인 신청**
{% endhint %}

**\[다운로드 워크플로우 화면 표시]**

다운로드 워크플로우가 생성된 경우, 신청자로 설정된 사용자가 파일을 다운로드하려고 하면 다운로드를 신청할 수 있는 "다운로드 워크플로우" 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1014).png" alt=""><figcaption></figcaption></figure>

다운로드 워크플로우에서 신청자로 설정되지 않은 사용자가 파일을 다운로드하려고 하면 다음 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1539).png" alt=""><figcaption></figcaption></figure>



**\[다운로드 신청]**

1. '다운로드 워크플로우' 화면에서 다음 설정을 지정하고 '신청' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1015).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="161">항목</th><th>설명</th></tr></thead><tbody><tr><td>우선도</td><td>신청의 우선순위로 '일반', '긴급'을 선택합니다.</td></tr><tr><td>결재자</td><td>다운로드 워크플로우에 설정된 결재자가 표시됩니다.<br>워크플로우에 참조자나 대리 결재자가 설정되어 있는 경우 ▼를 클릭하여 확인할 수 있습니다.<br>유효한 다운로드 워크플로우가 여러 개인 경우 워크플로우를 선택하여 결재자를 전환할 수 있습니다.</td></tr><tr><td>제목</td><td>신청서의 제목을 입력합니다.</td></tr><tr><td>다운로드 목록</td><td>다운로드를 신청한 파일 목록이 표시됩니다.</td></tr><tr><td>다운로드 만료일</td><td>체크를 하면 다운로드의 기한을 설정할 수 있습니다.<br>날짜 입력란을 클릭하고 표시된 캘린더에서 날짜를 클릭하면 기한이 설정됩니다.</td></tr></tbody></table>



2. 'Workflow' > '기안함' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1016).png" alt=""><figcaption></figcaption></figure>



3. 상태가 '대기'인 신청이 추가되어 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1017).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="129">항목</th><th>설명</th></tr></thead><tbody><tr><td>제목</td><td>신청의 제목이 표시됩니다.</td></tr><tr><td>기능</td><td><p>신청의 대상이 되는 기능이 표시됩니다.</p><ul><li>다운로드:<br>파일 다운로드</li><li>링크전송:<br>폴더 및 파일 링크 전송</li><li>파일첨부 메일발송:<br>첨부 파일 생성</li><li>업로드:<br>파일 업로드</li></ul></td></tr><tr><td>기안일</td><td>신청한 날짜와 시간이 표시됩니다.</td></tr><tr><td>결재자</td><td>신청서에 설정된 결재자가 표시됩니다.</td></tr><tr><td>결재일</td><td>신청이 승인된 날짜와 시간이 표시됩니다.</td></tr><tr><td>상태</td><td><p>신청 상태가 표시됩니다.</p><ul><li>대기:<br>결재자가 신청을 탐색하기 전의 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 있습니다.</li><li>회수:<br>신청자가 신청을 회한 상태입니다.</li><li>열람 중:<br>결재자가 신청을 열람한 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 없습니다.</li><li>반송:<br>워크플로우에 설정된 결재자가 한 명만 있는 경우 신청이 승인되기 전에 결재자의 사용자 ID가 DirectCloud에서 삭제된 상태입니다. 신청자는 다른 신청자를 재설정하여 '재신청'하거나 신청을 '취소'해야 합니다.</li><li>승인:<br>신청이 승인된 상태입니다.</li><li>거절:<br>신청이 거절된 상태입니다.</li></ul></td></tr></tbody></table>



**\[신청 승인 후 파일 다운로드]**

신청이 승인되면 파일을 다운로드할 수 있습니다.

1. 'Workflow' > '기안함' 메뉴에서 상태가 '승인'인 다운로드 신청을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1019).png" alt=""><figcaption></figcaption></figure>



2. 다운로드 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1020).png" alt=""><figcaption></figcaption></figure>



3. 다운로드하려는 파일을 체크하고 다운로드 버튼을 클릭합니다.\
   파일의 오른쪽 가장자리에 표시된 ▼ 버튼을 클릭하고 "다운로드"를 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1021).png" alt=""><figcaption></figcaption></figure>



**\[다운로드 신청이 거절된 경우]**

신청이 거절되었을 경우, 다운로드 워크플로우 화면에 표시되고 있는 메시지에 「ㅇㅇ님이 거절하였습니다.」의▼를 클릭하면, 결재자 또는 대리 결재자가 신청을 거절했을 때에 입력한 이유를 확인할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1022).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 다운로드 승인 신청**
{% endhint %}

**\[다운로드 신청 화면 표시]**

다운로드 워크플로우가 생성된 경우 신청자로 설정된 사용자가 파일을 다운로드하려고 하면 다운로드를 신청할 수 있는 "다운로드 워크플로우" 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1541).png" alt=""><figcaption></figcaption></figure>

다운로드 워크플로우에서 신청자로 설정되지 않은 사용자가 파일을 다운로드하려고 하면 다음 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1540).png" alt=""><figcaption></figcaption></figure>



**\[다운로드 신청]**

1. '다운로드 워크플로우' 화면에서 다음 설정을 지정하고 '신청' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1542).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="161">항목</th><th>설명</th></tr></thead><tbody><tr><td>우선도</td><td>신청의 우선순위로 '일반', '긴급'을 선택합니다.</td></tr><tr><td>결재자</td><td>다운로드 워크플로우에 설정된 결재자가 표시됩니다.<br>워크플로우에 참조자나 대리 결재자가 설정되어 있는 경우 ▼를 클릭하여 확인할 수 있습니다.<br>유효한 다운로드 워크플로우가 여러 개인 경우 워크플로우를 선택하여 결재자를 전환할 수 있습니다.</td></tr><tr><td>제목</td><td>신청서의 제목을 입력합니다.</td></tr><tr><td>다운로드 목록</td><td>다운로드를 신청한 파일 목록이 표시됩니다.</td></tr><tr><td>다운로드 만료일</td><td>체크를 하면 다운로드의 기한을 설정할 수 있습니다.<br>날짜 입력란을 클릭하고 표시된 캘린더에서 날짜를 클릭하면 기한이 설정됩니다.</td></tr></tbody></table>



2. 신청 완료 화면에서 OK 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1543).png" alt=""><figcaption></figcaption></figure>



3. DirectCloud 드라이브의 공유 폴더 등을 마우스 오른쪽 단추로 클릭하고 나타나는 메뉴에서 'DirectCloud -Drive' > '워크플로우'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1544).png" alt=""><figcaption></figcaption></figure>



4. 상태가 '대기'인 신청이 추가되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1545).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="129">항목</th><th>설명</th></tr></thead><tbody><tr><td>제목</td><td>신청의 제목이 표시됩니다.</td></tr><tr><td>기능</td><td><p>신청의 대상이 되는 기능이 표시됩니다.</p><ul><li>다운로드:<br>파일 다운로드</li><li>링크전송:<br>폴더 및 파일 링크 만들기</li><li>파일첨부 메일발송:<br>첨부 파일 생성</li><li>업로드:<br>파일 업로드</li></ul></td></tr><tr><td>기안일</td><td>신청한 날짜와 시간이 표시됩니다.</td></tr><tr><td>결재자</td><td>신청서에 설정된 결재자가 표시됩니다.</td></tr><tr><td>결재일</td><td>신청이 승인된 날짜와 시간이 표시됩니다.</td></tr><tr><td>상태</td><td><p>신청 상태가 표시됩니다.</p><ul><li>대기:<br>결재자가 신청을 탐색하기 전의 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 있습니다.</li><li>회수:<br>신청자가 신청을 회한 상태입니다.</li><li>열람 중:<br>결재자가 신청을 열람한 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 없습니다.</li><li>반송:<br>워크플로우에 설정된 결재자가 한 명만 있는 경우 신청이 승인되기 전에 결재자의 사용자 ID가 DirectCloud에서 삭제된 상태입니다. 신청자는 다른 신청자를 재설정하여 '재신청'하거나 신청을 '취소'해야 합니다.</li><li>승인:<br>신청이 승인된 상태입니다.</li><li>거절:<br>신청이 거절된 상태입니다.</li></ul></td></tr></tbody></table>



**\[신청 승인 후 파일 다운로드]**

신청이 승인되면 파일을 다운로드할 수 있습니다.

1. 워크플로우의 신청 목록에서 상태가 '승인'인 다운로드 신청을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1546).png" alt=""><figcaption></figcaption></figure>



2. 다운로드 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1547).png" alt=""><figcaption></figcaption></figure>



3. 다운로드하려는 파일을 체크하고 다운로드 버튼을 클릭합니다.\
   파일의 오른쪽 가장자리에 표시된 ▼ 버튼을 클릭하고 "다운로드"를 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1548).png" alt=""><figcaption></figcaption></figure>



**\[다운로드 신청이 거절된 경우]**

신청이 거절되었을 경우, 다운로드 워크플로우 화면에 표시되고 있는 메시지 「ㅇㅇ님이거절하였습니다.」의▼를 클릭하면, 결재자 또는 대리 결재자가 신청을 거절했을 때에 입력한 이유를 확인할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1549).png" alt=""><figcaption></figcaption></figure>
