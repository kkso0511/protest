---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/workflow/change_content_workflow
---

# 신청한 워크플로우의 내용을 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 워크플로우를 이용하면 사용자가 아래 작업을 수행할 때 결재자의 승인을 받도록 설정할 수 있습니다.

* 파일 다운로드
* 폴더 및 파일의 링크 생성
* 파일첨부 메일발송
* 파일 업로드

워크플로우 신청자로 지정된 사용자가 대상 기능을 사용하기 위해 승인 신청을 하고, 워크플로우 결재자로 지정된 사용자가 이를 승인함으로써 비로소 작업이 가능해지는 구조입니다.\
이 매뉴얼에서는 Web 브라우저와 DirectCloud 드라이브에서 이미 신청한 워크플로우의 내용을 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리 페이지에서 '워크플로우'가 '사용' 으로 활성화되어 있더라도, '공유설정'->' Shared Box 관리' 에서\
  '워크플로우'가 사용안함’으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
* 상태가 승인 대기 이외인 신청은 내용을 변경할 수 없습니다.
* 워크플로우에 설정된 결재자가 1명만 있는 경우, 결재가 이루어지기 전에 해당 결재자의 사용자 ID가 DirectCloud에서 삭제되면 신청 상태가 반려로 변경됩니다.\
  이 경우에는 다른 신청자를 다시 설정하여 재신청하시거나 신청 철회를 진행하셔야 합니다.
*   다음 작업이 수행되면 대리 결재자 또는 결재자에게 알림 메일이 발송됩니다.\
    단, 신청 내용 변경이나 신청 삭제의 경우에는 알림 메일이 발송되지 않습니다.

    * 신청자에 의한 승인 신청
    * 신청자에 의한 신청한 워크플로우의 철회
    * 대리 결재자 또는 결재자에 의한 워크플로우의 승인 또는 거절

    신청자에게는 다음 작업이 수행될 때 알림 메일이 발송됩니다.

    * 대리 결재자 또는 결재자에 의한 워크플로우의 승인 또는 거절
* 신청자로 등록된 Guest는 결재 신청, 내용 변경, 신청 철회, 삭제를 할 수 있습니다.
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

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 워크플로우 내용 변경**
{% endhint %}

워크플로우 신청자는 본인이 결재 요청을 제출한 이후, 결재자가 해당 신청을 확인하기 전까지는 신청 내용을 변경할 수 있습니다.

1. 'Workflow' > '기안함' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (822).png" alt=""><figcaption></figcaption></figure>



2. 상태가 '대기'인 신청을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (823).png" alt=""><figcaption></figcaption></figure>



3. 신청 설정을 변경하고 변경 버튼을 클릭합니다.\
   설정 항목에 대한 자세한 내용은 각 기능별 매뉴얼을 참조하십시오.

* [다운로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/download_workflow_apply)
* [링크전송 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/link_workflow_apply)
* [파일첨부 메일발송 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/mail_workflow_apply)
* [업로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/upload_workflow_apply)

단, 우선도와 결재자는 변경할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (827).png" alt=""><figcaption></figcaption></figure>



4. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>

신청 설정이 변경되고 '해당 워크플로우가 수정되었습니다.'라는 메시지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (829).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 워크플로우 내용 변경**
{% endhint %}

워크플로우 신청자는 본인이 결재 요청을 제출한 이후, 결재자가 해당 신청을 확인하기 전까지는 신청 내용을 변경할 수 있습니다.

1. DirectCloud 드라이브의 Shared Box 등에서 마우스 오른쪽 버튼을 클릭한 뒤 나타나는 메뉴에서 'DirectCloud-Drive' > '워크플로우'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (830).png" alt=""><figcaption></figcaption></figure>



2. 상태가 '대기'인 신청을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (831).png" alt=""><figcaption></figcaption></figure>



3.  신청 설정을 변경하고 변경 버튼을 클릭합니다.\
    설정 항목에 대한 자세한 내용은 각 기능별 매뉴얼을 참조하십시오.

    * [다운로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/download_workflow_apply)
    * [링크전송 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/link_workflow_apply)
    * [파일첨부 메일발송 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/mail_workflow_apply)
    * [업로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/workflow/upload_workflow_apply)

    단, 우선도와 결재자는 변경할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (824).png" alt=""><figcaption></figcaption></figure>



4. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (825).png" alt=""><figcaption></figcaption></figure>

신청 설정이 변경되고 '해당 워크플로우가 수정되었습니다.'라는 메시지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (832).png" alt=""><figcaption></figcaption></figure>
