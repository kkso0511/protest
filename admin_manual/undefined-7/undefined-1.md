---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-7/undefined-1
---

# 워크플로우를 관리하는 방법

### 개요 <a href="#a03" id="a03"></a>

워크플로우를 사용하면 사용자가 다음 작업을 수행할 때 결재자가 승인할 수 있도록 설정할 수 있습니다.

* 다운로드
* 링크전송
* 파일첨부 메일발송
* 업로드

워크플로우의 신청자로 지정된 사용자가 대상 기능을 이용하기 위한 승인 신청을 하고, 워크플로우의 결재자로 지정된 사용자에 의해 승인됨으로써, 비로소 조작이 가능해지는 구조입니다.\
이 매뉴얼에서는 '워크플로우' > '기본 설정' 메뉴에서, 생성된 워크플로우를 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '워크플로우' 항목을 사용할 수 있습니다.
* [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-7/undefined)에서 워크플로우가 활성화되어 있더라도, [특정 폴더에서 워크플로우를 활성화하 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-20)에서 '워크플로우' 설정이 '사용 안함'으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
* 사용자에 의한 신청 목록을 확인하는 방법에 대해서는, [워크플로우의 신청 목록을 확인하는 방법](https://help.directcloud.net/admin_manual/undefined-7/undefined-7)을 참조해 주시기 바랍니다.
*   워크플로우의 작성자에는 LDAP 연동 및 SAML 연동으로 불러온 사용자도 추가할 수 있습니다.

    Guest와 Connect User는 추가할 수 없습니다.
* 다운로드 워크플로우에서 신청자로 추가된 사용자는 폴더 다운로드를 할 수 없게 됩니다.\
  파일을 다운로드하려고 하면 워크플로우 신청 화면이 표시됩니다.
* 업로드 워크플로우에서 신청자로 추가된 사용자는 폴더 업로드를 할 수 없게 됩니다.\
  파일을 업로드하려고 하면 워크플로우 신청 화면이 표시됩니다.
*   다운로드·업로드 워크플로우에서 신청자로 추가된 사용자는 DirectCloud 드라이브에서 다음 작업을 수행할 수 없게 됩니다.

    * 드래그 앤 드롭으로 다운로드 및 업로드
    * 직접 편집
    * 폴더 및 파일 이름 변경
    * 폴더 및 파일 이동
    * 폴더 및 파일 복사
    * 폴더 생성
    * 폴더 및 파일 삭제

    자세한 내용은 [다운로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/undefined-9/undefined-3)과 [업로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/undefined-9/undefined-6)을 참고해 주세요.
* 링크 워크플로우를 생성한 경우, 신청자로 지정된 사용자는 링크 복사 및 외부 메일 프로그램을 통한 전송을 할 수 없게 됩니다. 자세한 내용은 [링크전송 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/undefined-9/undefined-4)을 참고해 주세요.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**워크플로우 관리**
{% endhint %}

1. '워크플로우' > '설정' 메뉴를 선택하고 '워크플로우 관리' 탭을 클릭합니다.\
   작성된 워크플로우 목록 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2188).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. 관리자 또는 사용자가 만든 워크플로우를 검토합니다.

<figure><img src="../../.gitbook/assets/image (2189).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="207">항목</th><th>설명</th></tr></thead><tbody><tr><td>결재선명</td><td>작성된 워크플로우의 이름이 표시됩니다.</td></tr><tr><td>기능</td><td><p>워크플로우의 대상이 되는 기능이 표시됩니다.<br>복수의 기능이 대상의 경우, '00(기능) 외 0건'이라고 표시됩니다.</p><ul><li>다운로드:<br>파일 다운로드</li><li>링크전송:<br>폴더 및 파일 링크 생성</li><li>파일첨부 메일발송:<br>파일첨부 메일 생성</li><li>업로드:<br>파일 업로드</li></ul></td></tr><tr><td>자동승인</td><td>워크플로우에 자동 승인이 설정되어 있으면 워크플로우가 자동으로 승인되기까지의 일수로 0~5일이 표시됩니다.</td></tr><tr><td>작성자</td><td>워크플로우를 만든 사용자의 이름이 표시됩니다.</td></tr><tr><td>최종수정일</td><td><p>워크플로우가 업데이트된 날짜와 시간으로 다음 중 하나가 표시됩니다.</p><ul><li>워크플로우가 생성된 날짜와 시간</li><li>워크플로우가 수정된 날짜와 시간</li></ul></td></tr><tr><td>상태</td><td><p>워크플로우의 상태로 다음 중 하나가 표시됩니다.</p><ul><li>사용</li><li>대기</li><li>삭제</li></ul></td></tr><tr><td>동작</td><td><p>[상세] 버튼을 클릭하면 [상세] 화면에 다음의 상세 정보가 표시됩니다.</p><ul><li><p>기본 정보</p><ul><li>결재선명</li><li>기능</li><li>작성자</li><li>상태</li></ul></li><li><p>결재선</p><ul><li>신청자</li><li>참조자</li><li>대리 결재자</li><li>결재자</li></ul></li></ul><p>또한 휴지통 버튼을 클릭하면 확인 화면에서 워크플로를 삭제할 수 있습니다.</p></td></tr></tbody></table>



{% hint style="warning" %}
**생성된 워크플로우를 필터링 해서 보기**
{% endhint %}

생성된 워크플로우 목록에서 상태, 기능, 결제선명, 사용자 이름 및 사용자 ID로 필터링하여 볼 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2190).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="72.79998779296875">No.</th><th width="604.800048828125">설명</th></tr></thead><tbody><tr><td>1</td><td>클릭하여 드롭다운 리스트를 표시하고, 생성된 워크플로우를 필터링하여 표시하고 싶은 상태를 선택합니다.</td></tr><tr><td>2</td><td>클릭하여 드롭다운 리스트를 표시하고, 생성된 워크플로우를 필터링하여 표시하고 싶은 기능을 선택합니다.</td></tr><tr><td>3</td><td>생성된 워크플로우를 워크플로우 이름이나 생성자로 필터링하는 경우, '워크플로우명' 또는 '사용자명', '사용자 ID' 중 하나를 입력합니다.</td></tr></tbody></table>
