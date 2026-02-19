---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/workflow/create_workflow
---

# 워크플로우를 생성하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 워크플로우를 이용하면 사용자가 아래 작업을 수행할 때 결재자의 승인을 받도록 설정할 수 있습니다.

* 파일 다운로드
* 폴더 및 파일의 링크 전송
* 파일첨부 메일발송
* 파일 업로드

워크플로우 신청자로 지정된 사용자가 대상 기능을 사용하기 위해 승인 신청을 하고, 워크플로우 결재자로 지정된 사용자가 이를 승인함으로써 비로소 작업이 가능해지는 구조입니다.\
이 매뉴얼 에서는 사용자 페이지에서 워크플로우를 생성하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 워크플로우를 생성하는 관리자는 관리 페이지에서 '결재선관리 담당자'로 설정되어 있어야 합니다.\
  자세한 내용은 [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)을 참조해주시기 바랍니다.
* 신청자, 참조자, 대리 결재자, 결재자를 일괄 추가하는 것은 불가능합니다.
* Guest는 신청자로 추가할 수 있지만, 참조자·대리 결재자·결재자로 추가할 수는 없습니다.
* 대리 결재자나 결재자에 그룹이 등록되어 있는 경우 승인 요청이 이루어지면 그룹에 속한 모든 사용자에게 승인 요청 알림 메일이 전송됩니다.
* 자동 결재에 체크한 경우 선택한 일수가 지난 뒤 0시 0분에 자동으로 승인됩니다.\
  단, 설정한 당일의 밤 0시 0분까지를 1일로 계산합니다.\
  예를 들어 2023년 8월 7일 13시에 설정하고 자동 결재를 1일로 설정한 경우, 다음 날인 2023년 8월 8일 0시 0분에 자동 결됩니다.
* 워크플로우는 특정 파일을 지정하여 적용할 수 없습니다.
* 다운로드 워크플로우에서 신청자로 설정된 사용자는 모바일 애플리케이션에서 파일을 다운로드할 수 없게 됩니다.
*   다운로드, 업로드 워크플로우에서 신청자로 설정된 사용자는 DirectCloud 드라이브에서 아래 작업을 수행할 수 없습니다.

    * 드래그 앤드 드롭으로 다운로드 및 업로드
    * 직접 편집
    * 이름 변경
    * 폴더와 파일 이동
    * 폴더와 파일 복사
    * 폴더 생성
    * 폴더와 파일 삭제

    아래 작업은 가능합니다.

    * 오른쪽 클릭 메뉴에서 다운로드 및 업로드
    * 미리보기
    * 온라인 편집
    * 링크 생성
    * 버전 관리
    * 파일 잠금
* 링크전송, 파일첨부 메일발송 워크플로우에서는 신청자에게 작업 제한이 적용되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**워크플로우에서 담당자의 역할**
{% endhint %}

워크플로우에서는 다음과 같은 여러 담당자를 구성할 수 있습니다.

<table><thead><tr><th width="138">담당자</th><th width="499">설명</th><th>필수여부</th></tr></thead><tbody><tr><td>신청자</td><td>워크플로우의 기능에 설정된 작업을 수행했을 때 워크플로우가 적용되는 그룹, 사용자, Guest입니다.</td><td>〇</td></tr><tr><td>참조자</td><td>'워크플로우' > '결재함' 메뉴를 열람할 수 있는 그룹, 사용자입니다.</td><td> </td></tr><tr><td>대리 결재자</td><td>결재자를 대신하여 결재할 수 있는 그룹, 사용자입니다.<br>결재자와 대리 결재자 중 한 명이라도 신청을 승인하면 상태가 승인으로 변경됩니다.</td><td> </td></tr><tr><td>결재자</td><td>신청자로부터의 요청을 승인할 수 있는 그룹, 사용자입니다.<br>결재자와 대리 결재자 중 한 명이라도 신청을 승인하면 상태가 승인으로 변경됩니다.</td><td>〇</td></tr></tbody></table>



{% hint style="warning" %}
**워크플로우 생성하기**
{% endhint %}

1. 'Workflow' > '결재선' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (990).png" alt=""><figcaption></figcaption></figure>



2. 결재선 생성 버튼을 클릭합니다.\
   새 워크플로 만들기 화면이 표시됩니다.



3. '기본 정보'를 설정합니다.

<figure><img src="../../.gitbook/assets/image (992).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="167">항목</th><th width="473">설명</th><th>필수 여부</th></tr></thead><tbody><tr><td>상태</td><td><p>워크플로우의 상태로 다음 중 하나를 선택합니다.</p><ul><li>사용</li><li>대기</li></ul></td><td>〇</td></tr><tr><td>기능</td><td><p>워크플로우의 대상이 되는 기능을 체크합니다.</p><p></p><ul><li>파일 다운로드: 파일 다운로드</li><li>링크 전송: 폴더 및 파일 링크 생성</li><li>파일첨부 메일발송: 파일을 첨부하여 이메일 발송</li><li>업로드: 파일 업로드</li></ul></td><td>〇</td></tr><tr><td>결재선 명</td><td>만들 워크플로우의 이름을 입력합니다.</td><td>〇</td></tr></tbody></table>



4. 워크플로우 설정에서 신청자를 설정합니다.

❶ 추가 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (993).png" alt=""><figcaption></figcaption></figure>

❷ 신청자에게 그룹을 추가하려면 '그룹으로 추가'를 선택하고 그룹 트리에서 신청자에게 추가할 그룹을 선택한 다음 추가 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (994).png" alt=""><figcaption></figcaption></figure>

❸ 신청자에 사용자를 추가하려면 '사용자로 추가'를 선택하고, 추가할 사용자를 선택 후 추가 버튼을 클릭합니다. 이때 그룹 트리에서 그룹을 선택하여 사용자를 좁힐 수 있습니다. 또한 이름이나 ID로 검색할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (995).png" alt=""><figcaption></figcaption></figure>

&#x20;  그룹 트리에서 ◯◯ Guest를 선택하여 Guest를 추가할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (996).png" alt=""><figcaption></figcaption></figure>



5. 워크플로우 설정에서 결재자를 설정합니다.\
   결재자의 추가 버튼을 클릭하고 4단계와 동일한 방법으로 결재자를 추가합니다.

<figure><img src="../../.gitbook/assets/image (2495).png" alt="" width="563"><figcaption></figcaption></figure>



6. 필요한 경우 참조자 및 대리 결재자를 추가합니다.

❶ 참조자 및 대리 결재자를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (997).png" alt=""><figcaption></figcaption></figure>

❷ 참조자 또는 대리 결재자의 추가 버튼을 클릭하고 4단계와 동일한 방법으로 참조자 또는 대리 결재자를 추가합니다.

<figure><img src="../../.gitbook/assets/image (998).png" alt=""><figcaption></figcaption></figure>



7. 자동 결재를 설정하려면 '자동 결재'를 선택하고 자동 결재까지의 일 수를 선택합니다.

<figure><img src="../../.gitbook/assets/image (999).png" alt=""><figcaption></figcaption></figure>



8. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1000).png" alt=""><figcaption></figcaption></figure>



9. 워크플로우가 작성됩니다.

<figure><img src="../../.gitbook/assets/image (1001).png" alt=""><figcaption></figcaption></figure>
