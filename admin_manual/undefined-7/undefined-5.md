---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-7/undefined-5
---

# 삭제된 워크플로우를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

워크플로우를 사용하면 사용자가 다음 작업을 수행할 때 결재자가 승인할 수 있도록 설정할 수 있습니다.

* 다운로드
* 링크전송
* 파일첨부 메일발송
* 업로드

워크플로우의 신청자로 지정된 사용자가 대상 기능을 이용하기 위한 승인 신청을 하고, 워크플로우의 결재자로 지정된 사용자에 의해 승인됨으로써, 비로소 조작이 가능해지는 구조입니다.\
이 매뉴얼에서는 '워크플로우' > '설정' 메뉴에서, 삭제된 워크플로우를 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '워크플로우' 항목을 사용할 수 있습니다.
* 워크플로우를 이용하려면 [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-7/undefined)의 절차에 따라, '워크플로우 설정'에서 '사용'이 선택되어 있어야 합니다.
* [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-7/undefined)에서 워크플로우가 활성화되어 있더라도, [특정 폴더에서 워크플로우를 활성화하 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-20)에서 '워크플로우' 설정이 '사용 안함'으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
* 사용자에 의해 신청된 워크플로우를 확인하는 방법에 대해서는, [워크플로우 신청 목록을 확인하는 방법](https://help.directcloud.net/admin_manual/undefined-7/undefined-6)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '워크플로우' > '설정' 메뉴를 선택하고 '삭제된 워크플로우 현황' 탭을 클릭합니다.\
   삭제된 워크플로우의 목록이 나타납니다.

<figure><img src="../../.gitbook/assets/image (2087).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. 관리자 또는 사용자가 삭제한 워크플로우를 확인합니다.

<figure><img src="../../.gitbook/assets/image (2088).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="195">항목</th><th>설명</th></tr></thead><tbody><tr><td>결재선명</td><td>삭제된 워크플로우의 이름이 표시됩니다.</td></tr><tr><td>기능</td><td><p>워크플로우의 대상이 되는 기능이 표시됩니다.<br>복수의 기능이 대상의 경우, '00(기능) 외 0건'이라고 표시됩니다.</p><ul><li>다운로드:<br>파일 다운로드</li><li>링크전송:<br>폴더 및 파일 링크 생성</li><li>파일첨부 메일발송:<br>파일첨부 메일 생성</li><li>업로드:<br>파일 업로드</li></ul></td></tr><tr><td>자동승인</td><td>삭제된 워크플로에 자동 승인이 설정되어 있으면 워크플로우가 자동으로 승인되기까지의 일수로 1~5가 표시됩니다.<br>0일이 설정되어 있으면 "즉시"가 표시됩니다.</td></tr><tr><td>작성자</td><td>워크플로우의 '작성자'에 표시되어 있던 사용자의 이름이 표시됩니다.</td></tr><tr><td>최종수정일</td><td>워크플로우가 삭제된 날짜와 시간이 표시됩니다.</td></tr><tr><td>상태</td><td>워크플로우의 상태로, '삭제'라고 표시됩니다.</td></tr></tbody></table>
