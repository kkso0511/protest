---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-9/undefined-12
---

# 파일첨부 메일발송 신청을 승인하거나 거부하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 워크플로우를 이용하면 사용자가 아래 작업을 수행할 때 결재자의 승인을 받도록 설정할 수 있습니다.

* 파일 다운로드
* 폴더 및 파일의 링크 생성
* 파일첨부 메일발송
* 파일 업로드

워크플로우 신청자로 지정된 사용자가 대상 기능을 사용하기 위해 승인 신청을 하고, 워크플로우 결재자로 지정된 사용자가 이를 승인함으로써 비로소 작업이 가능해지는 구조입니다.\
이 매뉴얼에서는 Web 애플리케이션과 DirectCloud 드라이브에서 파일첨부 메일발송 신청을 승인하거나 거부하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리 페이지에서 '워크플로우'가 '사용' 으로 활성화되어 있더라도, '공유설정'->' Shared Box 관리' 에서\
  '워크플로우'가 사용안함’으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
* 대리 결재자 또는 결재자로 설정된 워크플로우가 있는 경우, ‘Workflow’ ＞ ‘결재함’ 메뉴가 표시됩니다.
*   다음 작업이 수행되면 대리 결재자 또는 결재자에게 알림 메일이 발송됩니다.\
    단, 신청 내용 변경이나 신청 삭제의 경우에는 알림 메일이 발송되지 않습니다.

    * 신청자에 의한 승인 신청
    * 신청자에 의한 신청한 워크플로우의 철회
    * 대리 결재자 또는 결재자에 의한 워크플로우의 승인 또는 거절

    신청자에게는 다음 작업이 수행될 때 알림 메일이 발송됩니다.

    * 대리 결재자 또는 결재자에 의한 워크플로우의 승인 또는 거절
* 대리 결재자 또는 결재자에 그룹이 등록되어 있는 경우,\
  승인 요청이 제출되면 그룹에 속한 모든 사용자의 이메일 주소로 승인 요청 알림 메일이 발송됩니다.
*   워크플로우 설정에서 ‘자동 승인’에 체크되어 있는 경우,  선택한 일수가 경과한 후 0시 0분에 자동으로 승인됩니다.\
    단, 설정한 날의 자정(0시 0분)까지를 하루로 계산합니다.

    예를 들어, 설정일이 2023년 8월 7일 13시이고 자동 승인을 1일로 설정한 경우, 그날 밤 2023년 8월 8일 0시 0분에 자동 승인됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 파일첨부 메일발송 워크플로우 승인/거절**
{% endhint %}

**\[파일첨부 메일발송 승인 화면 표시]**

1. 파일첨부 메일발송 워크플로우의 결재자 또는 대리 결재자로 설정된 사용자로 사용자 페이지에 로그인합니다.\
   승인/거절이 필요한 신청이 있는 경우, '결재함' 메뉴의 오른쪽 상단에 빨간색 둥근 숫자로 표시됩니다.



2. Workflow > 결재함 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (913).png" alt=""><figcaption></figcaption></figure>

자신이 결재자 또는 대리 결재자로 설정된 워크플로우의 신청 목록이 표시됩니다.\
승인/거절이 필요한 신청은 굵게 표시되어 있습니다.

<figure><img src="../../.gitbook/assets/image (914).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="129">항목</th><th>설명</th></tr></thead><tbody><tr><td>제목</td><td>신청의 제목이 표시됩니다.</td></tr><tr><td>기능</td><td><p>신청의 대상이 되는 기능이 표시됩니다.</p><ul><li>다운로드:<br>파일 다운로드</li><li>링크전송:<br>폴더 및 파일 링크 만들기</li><li>파일첨부 메일발송:<br>첨부 파일 생성</li><li>업로드:<br>파일 업로드</li></ul></td></tr><tr><td>신청자</td><td>워크플로우를 신청한 사람의 이름이 표시됩니다.</td></tr><tr><td>기안일</td><td>신청한 날짜와 시간이 표시됩니다.</td></tr><tr><td>결재자</td><td>신청서에 설정된 결재자가 표시됩니다.</td></tr><tr><td>결재일</td><td>신청이 승인된 날짜와 시간이 표시됩니다.</td></tr><tr><td>상태</td><td><p>신청 상태가 표시됩니다.</p><ul><li>대기:<br>결재자가 신청을 탐색하기 전의 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 있습니다.</li><li>회수:<br>신청자가 신청을 회한 상태입니다.</li><li>열람 중:<br>결재자가 신청을 열람한 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 없습니다.</li><li>반송:<br>워크플로에 설정된 결재자가 한 명만 있는 경우 신청이 승인되기 전에 결재자의 사용자 ID가 DirectCloud에서 삭제된 상태입니다. 신청자는 다른 신청자를 재설정하여 '재신청'하거나 신청을 '취소'해야 합니다.</li><li>승인:<br>신청이 승인된 상태입니다.</li><li>거절:<br>신청이 거절된 상태입니다.</li></ul></td></tr></tbody></table>



3. 승인/거절할 신청을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (915).png" alt=""><figcaption></figcaption></figure>

파일첨부 메일발송 워크플로우 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (916).png" alt=""><figcaption></figcaption></figure>



**\[파일첨부 메일발송이 신청된 파일 확인]**

1. 파일첨부 메일발송 워크플로우 화면에서 파일검토를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (917).png" alt=""><figcaption></figcaption></figure>

파일첨부 메일발송이 신청된 파일 목록이 표시됩니다.\
파일첨부 메일발송을 신청하는 파일 목록은 '파일검토'을 클릭한 승인자만 확인할 수 있습니다. 보안상 파일 확인 화면의 URL은 다른 사용자와 공유할 수 없습니다.



2. 파일을 다운로드하려면 확인란을 선택하고 다운로드 버튼을 클릭합니다.\
   파일의 오른쪽 가장자리에 표시된 ▼ 버튼을 클릭하고 "다운로드"를 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (918).png" alt=""><figcaption></figcaption></figure>



3. 파일 내용을 온라인으로 확인하려면 파일 이름을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (919).png" alt=""><figcaption></figcaption></figure>

미리보기 화면에 파일이 표시됩니다.\
이 화면에서 오른쪽 상단의 다운로드 버튼을 클릭하여 파일을 다운로드할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (920).png" alt=""><figcaption></figcaption></figure>



**\[파일첨부 메일발송 신청 승인]**

1. 파일첨부 메일발송 워크플로우 화면에서 첨부파일 제출 신청 내용을 확인합니다.

<figure><img src="../../.gitbook/assets/image (921).png" alt=""><figcaption></figcaption></figure>

| 항목  | 설명                                     |
| --- | -------------------------------------- |
| 우선도 | 신청자가 설정한 신청의 우선순위로 ‘일’ 또는 ‘긴급’이 표시됩니다. |
| 신청자 | 파일첨부 메일발송 신청자가 표시됩니다.                  |
| 결재자 | 파일첨부 메일발송 워크플로우에 설정된 결재자가 표시됩니다.       |



2. 파일첨부 메일발송 설정을 검토하고 승인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (922).png" alt=""><figcaption></figcaption></figure>



3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (923).png" alt=""><figcaption></figcaption></figure>

신청이 승인되고 '해당 워크플로우가 승인되었습니다.'라는 메시지가 표시됩니다.\
또한 상태가 '승인'으로 변경됩니다.

<figure><img src="../../.gitbook/assets/image (924).png" alt=""><figcaption></figcaption></figure>



**\[파일첨부 메일발송 신청 거절]**

1. 파일첨부 메일발송 워크플로우 화면에서 첨부파일 제출 신청 내용을 확인하고 거절 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (925).png" alt=""><figcaption></figcaption></figure>



2. 거절 이유를 입력하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (926).png" alt=""><figcaption></figcaption></figure>

신청이 거부되고 "해당 워크플로우가 거절되었습니다."라는 메시지가 표시됩니다.\
또한 상태가 '거절'로 변경됩니다.

<figure><img src="../../.gitbook/assets/image (927).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 파일첨부 메일발송 워크플로우 승인/거절**
{% endhint %}

**\[파일첨부 메일발송 승인 화면 표시]**

1. 파일첨부 메일발송 워크플로우의 결재자 또는 대리 결재자로 구성된 사용자로 DirectCloud 드라이브에 로그인합니다.
2. DirectCloud 드라이브의 Shared Box 폴더 등을 마우스 오른쪽 단추로 클릭하고 나타나는 메뉴에서 'DirectCloud-Drive' > '워크플로우'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (928).png" alt=""><figcaption></figcaption></figure>

&#x20;      워크플로우의 신청 목록이 표시됩니다.



3. '결재함'을 클릭합니다.\
   자신이 결재자 또는 대리 결재자로 설정된 워크플로우의 신청 목록이 표시됩니다.\
   승인/거절이 필요한 신청은 굵게 표시되어 있습니다.

<figure><img src="../../.gitbook/assets/image (929).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="129">항목</th><th>설명</th></tr></thead><tbody><tr><td>제목</td><td>신청의 제목이 표시됩니다.</td></tr><tr><td>기능</td><td><p>신청의 대상이 되는 기능이 표시됩니다.</p><ul><li>다운로드:<br>파일 다운로드</li><li>링크전송:<br>폴더 및 파일 링크 만들기</li><li>파일첨부 메일발송:<br>첨부 파일 생성</li><li>업로드:<br>파일 업로드</li></ul></td></tr><tr><td>신청자</td><td>워크플로우를 신청한 사람의 이름이 표시됩니다.</td></tr><tr><td>기안일</td><td>신청한 날짜와 시간이 표시됩니다.</td></tr><tr><td>결재자</td><td>신청서에 설정된 결재자가 표시됩니다.</td></tr><tr><td>결재일</td><td>신청이 승인된 날짜와 시간이 표시됩니다.</td></tr><tr><td>상태</td><td><p>신청 상태가 표시됩니다.</p><ul><li>대기:<br>결재자가 신청을 탐색하기 전의 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 있습니다.</li><li>회수:<br>신청자가 신청을 회한 상태입니다.</li><li>열람 중:<br>결재자가 신청을 열람한 상태입니다. 신청자는 신청 내용의 변경과 철회를 할 수 없습니다.</li><li>반송:<br>워크플로에 설정된 결재자가 한 명만 있는 경우 신청이 승인되기 전에 결재자의 사용자 ID가 DirectCloud에서 삭제된 상태입니다. 신청자는 다른 신청자를 재설정하여 '재신청'하거나 신청을 '취소'해야 합니다.</li><li>승인:<br>신청이 승인된 상태입니다.</li><li>거절:<br>신청이 거절된 상태입니다.</li></ul></td></tr></tbody></table>



4. 승인/거절할 신청을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (930).png" alt=""><figcaption></figcaption></figure>

파일첨부 메일발송 워크플로우 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (931).png" alt=""><figcaption></figcaption></figure>



**\[파일첨부 메일발송이 신청된 파일 확인]**

1. 파일첨부 메일발송 워크플로우 화면에서 파일검토를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (932).png" alt=""><figcaption></figcaption></figure>

파일첨부 메일발송이 신청된 파일 목록이 표시됩니다.



2. 파일을 다운로드하려면 확인란을 선택하고 다운로드 버튼을 클릭합니다.\
   파일의 오른쪽 가장자리에 표시된 ▼ 버튼을 클릭하고 "다운로드"를 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (933).png" alt=""><figcaption></figcaption></figure>



3. 파일 내용을 온라인으로 확인하려면 파일 이름을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (934).png" alt=""><figcaption></figcaption></figure>

미리보기 화면에 파일이 표시됩니다.\
이 화면에서 오른쪽 상단의 다운로드 버튼을 클릭하여 파일을 다운로드할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (935).png" alt=""><figcaption></figcaption></figure>



**\[파일첨부 메일발송 신청 승인]**

1. 파일첨부 메일발송 워크플로우 화면에서 첨부파일 제출 신청 내용을 확인합니다.

<figure><img src="../../.gitbook/assets/image (936).png" alt=""><figcaption></figcaption></figure>

| 항목  | 설명                                     |
| --- | -------------------------------------- |
| 우선도 | 신청자가 설정한 신청의 우선순위로 ‘일’ 또는 ‘긴급’이 표시됩니다. |
| 신청자 | 파일첨부 메일발송 신청자가 표시됩니다.                  |
| 결재자 | 파일첨부 메일발송 워크플로우에 설정된 결재자가 표시됩니다.       |



2. 파일첨부 메일발송 설정을 검토하고 승인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (937).png" alt=""><figcaption></figcaption></figure>



3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (938).png" alt=""><figcaption></figcaption></figure>

신청이 승인되고 '해당 워크플로우가 승인되었습니다.'라는 메시지가 표시됩니다.\
또한 상태가 '승인'으로 변경됩니다.

<figure><img src="../../.gitbook/assets/image (939).png" alt=""><figcaption></figcaption></figure>



**\[파일첨부 메일발송 신청 거절]**

1. 파일첨부 메일발송 워크플로우 화면에서 첨부파일 제출 신청 내용을 확인하고 거절 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (940).png" alt=""><figcaption></figcaption></figure>



2. 거절 이유를 입력하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (941).png" alt=""><figcaption></figcaption></figure>

신청이 거부되고 "해당 워크플로우가 거절되었습니다."라는 메시지가 표시됩니다.\
또한 상태가 '거절'로 변경됩니다.

<figure><img src="../../.gitbook/assets/image (942).png" alt=""><figcaption></figcaption></figure>
