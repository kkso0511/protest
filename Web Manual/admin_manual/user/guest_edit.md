---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/guest_edit
---

# 관리자 페이지에서 Guest 정보를 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 'Guest' 관리 메뉴에서, 등록된 Guest 정보를 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* 사용자 목록은 등록일 기준으로 최신 순으로 표시되며, 정렬 방식은 변경할 수 없습니다.
* 동일한 이메일 주소로 여러 개의 사용자 ID를 생성할 수는 없습니다.
* Guest에게는 ‘보안 정책’ > ‘사용권한’ 메뉴의 설정이 적용되지 않기 때문에, 사용 권한 설정 항목이 없습니다.\
  다만, [Guest의 링크 생성 가능 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/user/guest_link_permission)을 통해 모든 Guest에 대해 링크 생성 허용 여부를 설정할 수는 있습니다.
* Guest ID는 한 번 설정하면 관리 페이지에서 변경할 수 없습니다.
* Guest 정보 수정 내용이 반영되지 않는 경우에는 web 브라우저 캐시를 삭제한 뒤 다시 수정해 주시기 바랍니다.
* Guest가 삭제되면 해당 Guest ID는 다시 재사용할 수 있게 됩니다.
* Guest 관리 메뉴에서는 그룹을 생성할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '계정 관리' > 'Guest' 메뉴를 선택하고 'Guest 관리' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1751).png" alt=""><figcaption></figcaption></figure>



2. 편집하려는 Guest의 동작 열에 표시되는 편집 버튼을 클릭합니다.\
   Guest 변경 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1752).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. Guest 정보를 편집하고 수정 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1753).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="151">항목</th><th>설명</th></tr></thead><tbody><tr><td>회사명</td><td>Guest가 속한 회사명을 250자 이내로 설정합니다.<br>사용 가능한 문자: 한자, 한글, 영숫자 기호</td></tr><tr><td>아이디</td><td>로그인할 때 Guest를 식별하는 데 사용되는 ID로 이메일 주소를 6~250자 이내로 설정합니다.<br>사용 가능한 문자: 영숫자, 기호(-_@.+#)</td></tr><tr><td>이름</td><td>Guest의 표시 이름을 250자 이내로 설정합니다.<br>사용 가능한 문자: 한자, 한글, 영숫자 기호</td></tr><tr><td>비밀번호</td><td><ul><li>비밀번호가 이미 등록되어 있는 경우에는 ‘등록 완료’라고 표시됩니다.<br>‘안내메일 재발송’ 버튼을 클릭하면, 비밀번호를 설정하기 위한 메일이 Guest의 사용자 ID로 설정된 이메일 주소로 전송됩니다.</li><li>비밀번호가 아직 등록되어 있지 않은 경우에는<br>‘등록용 메일 재전송’ 체크박스를 선택한 후 ‘저장’ 버튼을 클릭하면, 비밀번호 등록용 메일을 Guest에게 다시 보낼 수 있습니다.</li><li>‘링크 복사’ 버튼을 클릭하면 비밀번호 등록 화면의 URL이 복사됩니다.<br>비밀번호 등록용 URL의 유효 기간은 복사한 시점부터 24시간입니다.</li></ul></td></tr><tr><td>휴대전화</td><td>휴대전화 번호를 50자 이내로 설정합니다.<br>사용 가능한 문자: 숫자, 기호(+-)</td></tr><tr><td>언어</td><td><p>다음 언어를 설정합니다.</p><ul><li>사용자 페이지의 표시 언어</li><li>사용자에게 보내는 알림 메일</li></ul><p>사용자 페이지의 표시 언어를 변경하는 방법의 단계에 따라 Guest 자체에서 설정할 수도 있습니다.</p></td></tr><tr><td>GMT 변경</td><td>Guest의 시간대를 설정합니다.</td></tr><tr><td>상태</td><td>Guest를 활성 또는 비활성 상태로 설정할 수 있습니다.</td></tr><tr><td>사용권한</td><td><p>접근 가능한 폴더에 관한 다음 정보가 표시됩니다.</p><p></p><ul><li>폴더<br>접근 가능한 폴더의 경로가 표시됩니다.</li><li>초대자:<br>현재 선택한 Guest를 초대한 사용자가 표시됩니다.</li><li>등록일:<br>해당 폴더에 대한 접근이 가능해진 일시가 표시됩니다.</li><li>유효 기간:<br>해당 폴더에 접근할 수 있는 기간을 확인하고 변경할 수 있습니다.</li><li>권한:<br>해당 폴더에 설정된 접근 권한을 확인하고 변경할 수 있습니다.</li><li>메모:<br>Guest를 초대한 사용자가 메모에 입력한 내용이 표시됩니다.</li><li>삭제:<br>해당 폴더에 설정된 접근 권한을 해제할 수 있습니다.</li></ul></td></tr><tr><td>접속제어</td><td>Guest에게 '응용 프로그램', '장치 관리', '이중 인증', 'IP 제한'를 통한 접속 제어를 적용합니다.<br>여기에서는 '기본 설정' 또는 '개별 설정'을 선택합니다.<br>설정편집 버튼을 클릭하면 '보안 정책' > '접속 제어 개별설정' 메뉴로 이동합니다.</td></tr></tbody></table>
