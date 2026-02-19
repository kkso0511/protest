---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/connect_approve
---

# Connect User 초대를 승인하는 방법

### 개요 <a href="#a03" id="a03"></a>

Connect는 DirectCloud 회사 ID를 보유한 테넌트 간에 지정한 폴더를 공유할 수 있는 기능입니다.\
[관리자 승인 후 Connect 초대 메일을 발송하도록 설정하는 방법](https://help.directcloud.net/admin_manual/user/connect_admin_approval)의 절차에 따라 관리자에 의한 Connect 초대 승인이 활성화되어 있는 경우, ‘Connect User’ 메뉴의 ‘Connect User 승인’ 탭에서 승인 처리를 할 수 있습니다.\
이 매뉴얼에서는 관리자가 Connect User 초대를 승인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* Connect User 초대는 Guest 초대와 달리, 초대받는 사용자가 DirectCloud 회사 ID를 보유하고 있어야 합니다.
* 초대받는 테넌트에서는 다른 회사의 DirectCloud 사용자로부터 Connect User 초대를 받을 수 있도록, '공유 설정'->'세부 기능 설정' 항목에서 'Connect 연결'을 '사용'으로 설정해야 합니다.
* 아래 설정 항목은 초대받는 회사 ID의 보안 정책을 따르기 때문에, Connect User에는 적용되지 않습니다.
  * 비밀번호 정의
  * 정책 위반 발생 시 대응
  * 동시 로그인 제한
  * 자동 로그아웃
  * 로그인 알림
  * 애플리케이션 사용 제한
  * 기기 관리
  * 2단계 인증
  * 사용자 IP 주소 제한
  * 확장자 제한
  * 기능 제한
  * 링크 옵션 설정
  * 파일첨부 메일발송 시 비밀번호 설정
  * 업로드 요청 비밀번호 설정
  * 비밀번호 메일 발송
  * 모바일 앱 보안 설정

***

### 절차

1. ‘계정 관리’ > ‘Connect User’ 메뉴를 선택한 후, ‘Connect User 승인’ 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>



2. 사용자가 Connect User를 초대하면, ‘Connect User 초대’에 Connect User 초대와 관련된 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="210.800048828125">항목</th><th>내용</th></tr></thead><tbody><tr><td>초대자</td><td>Connect User를 초대한 사용자가 ‘사용자명(사용자 ID)’ 형식으로 표시됩니다.</td></tr><tr><td>초대받은 Connect User</td><td>Connect User 초대 메일을 받는 대상이 표시됩니다.<br>Connect User는 ‘회사 ID’와 ‘메일 주소’의 조합으로 관리되기 때문에, 회사 ID가 다를 경우 동일한 메일 주소를 사용할 수 있습니다.</td></tr><tr><td>신청일</td><td>Connect User 초대를 신청한 날짜와 시간이 표시됩니다.</td></tr><tr><td>유효기간</td><td>Connect User로 사용자 페이지에 로그인할 수 있는 유효기간이 표시됩니다.</td></tr><tr><td>정보</td><td>버튼을 클릭하면 ‘Connect User 초대 정보’ 화면에서 초대된 폴더나 메모 등을 확인할 수 있습니다.</td></tr><tr><td>상태</td><td><p>Connect User 초대의 승인 상태가 표시됩니다.</p><ul><li>승인 대기:<br>관리자 승인을 기다리는 상태입니다. ‘승인’ 버튼과 ‘거절’ 버튼이 표시됩니다.</li><li>승인:<br>관리자 승인이 완료된 상태입니다. 아직 Connect User의 등록은 완료되지 않은 상태입니다.</li><li>거절:<br>관리자에 의해 Connect User 초대가 거부된 상태입니다.</li><li>등록 완료:<br>관리자 승인과 Connect User의 등록이 모두 완료된 상태입니다.</li></ul></td></tr></tbody></table>



3. ‘상태’ 열의 ‘승인’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>



4. 확인 화면에서 ‘확인 버튼’을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>



5. '상태'열이 '승인'으로 변경되는 것을 확인합니다.

<figure><img src="../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

Connect User 등록이 완료되면 상태가 '등록 완료'로 변경됩니다.
