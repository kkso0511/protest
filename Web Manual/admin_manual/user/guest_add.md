---
metaLinks:
  alternates:
    - https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/guest_add
---

# 관리자 페이지에서 Guest를 추가하는 방법

### 개요 <a href="#a03" id="a03"></a>

사용자가 Guest를 초대하는 방식 외에도 관리자가 직접 Guest를 추가할 수 있습니다.\
이 매뉴얼에서는 관리 페이지의 '계정 관리 '메뉴에서 Guest를 직접추가하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* 사용자 목록은 등록일 기준 내림차순으로 표시됩니다. 정렬 순서를 변경할 수는 없습니다.
* 같은 이메일 주소를 사용하여 여러 개의 사용자 ID를 생성할 수는 없습니다.
* Guest에게는 ‘보안 정책’ > ‘사용권한’ 메뉴의 설정이 적용되지 않기 때문에, 사용 권한 설정 항목이 없습니다.\
  다만, [Guest의 링크 생성 가능 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/user/guest_link_permission)을 통해 모든 Guest에 대해 링크 생성 허용 여부를 설정할 수는 있습니다.
* Guest ID는 한 번 설정하면 관리자 페이지에서 변경할 수 없습니다.
* Guest가 삭제되면 해당 Guest의 ID는 다시 사용할 수 있게 됩니다.
* ‘Guest 관리’ 메뉴에서는 그룹을 생성할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '계정 관리' > 'Guest' 메뉴를 선택하고 'Guest 관리' 탭을 클릭한 다음 'Guest 추가' 버튼을 클릭합니다.\
   Guest 추가 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1749).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. Guest 정보를 입력하고 등록 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1750).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="151">항목</th><th>설명</th></tr></thead><tbody><tr><td>회사명</td><td>Guest가 속한 회사명을 250자 이내로 설정합니다.<br>사용 가능한 문자: 한자, 한글, 영숫자 기호</td></tr><tr><td>아이디</td><td>로그인할 때 Guest를 식별하는 데 사용되는 ID로 이메일 주소를 6~250자 이내로 설정합니다.<br>사용 가능한 문자: 영숫자, 기호(-_@.+#)</td></tr><tr><td>이름</td><td>Guest의 표시 이름을 250자 이내로 설정합니다.<br>사용 가능한 문자: 한자, 한글, 영숫자 기호</td></tr><tr><td>비밀번호</td><td>"비밀번호 등록 이메일 보내기"를 체크하고 "등록" 버튼을 클릭하면 패스워드 등록 이메일이 Guest 사용자 ID로 설정된 이메일 주소로 전송됩니다.</td></tr><tr><td>휴대전화</td><td>휴대전화 번호를 50자 이내로 설정합니다.<br>사용 가능한 문자: 숫자, 기호(+-)</td></tr><tr><td>언어</td><td><p>다음 언어를 설정합니다.</p><ul><li>사용자 페이지의 표시 언어</li><li>사용자에게 보내는 알림 메일</li></ul><p>사용자 페이지의 표시 언어를 변경하는 방법의 단계에 따라 Guest 자체에서 설정할 수도 있습니다.</p></td></tr><tr><td>GMT 변경</td><td>Guest의 시간대를 설정합니다.</td></tr><tr><td>접속제어</td><td>Guest에게 '접속 프로그램', '신규기기 승인', '2단계 인증', '사용자IP 제한'를 통한 접속 제어를 적용합니다.<br>여기에서는 "기본 설정" 또는 "개별 설정"을 선택합니다.<br>설정편집 버튼을 클릭하면 보안 정책 > 접속 제어 개별설정 메뉴로 이동합니다.</td></tr></tbody></table>
