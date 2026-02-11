---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-3/connect-user-3
---

# 등록된 Connect User의 정보를 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

Connect는 DirectCloud 회사 ID를 보유한 테넌트 간에 지정한 폴더를 공유할 수 있는 기능입니다.\
이 매뉴얼에서는 ‘Connect User’ 메뉴에서 등록된 Connect User의 정보를 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* Connect User 초대는 Guest 초대와 달리, 초대받는 사용자가 DirectCloud 회사 ID를 보유하고 있어야 합니다.
* 초대받는 테넌트에서는 다른 회사의 DirectCloud 사용자로부터 Connect User 초대를 받을 수 있도록, '공유 설정'->'세부 기능 설정' 항목에서 'Connect 연결'을 '사용'으로 설정해야 합니다.
* Connect User는 CSV 파일로 일괄 편집할 수 없습니다.
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
* ‘Connect User’ 메뉴의 ‘Connect User 관리’ 탭에서 변경할 수 있는 Connect User 정보는 ‘상태’, ‘유효기간’, ‘접근 권한’이며, 삭제할 수 있는 Connect User 정보는 ‘접근 권한’만 가능합니다.

***

### 절차

1. ‘계정 관리’ > ‘Connect User’ 메뉴를 선택한 후, ‘Connect User 관리’ 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>



2. 편집하려는 Connect User의 ‘동작’ 열에 표시된 편집 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2521).png" alt=""><figcaption></figcaption></figure>



3. Connect User 정보를 편집한 후 ‘수정’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2522).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="205.199951171875">항목</th><th>설명</th></tr></thead><tbody><tr><td>회사명</td><td>Connect User가 소속된 회사명이 표시됩니다.<br>회사명은 변경할 수 없습니다.</td></tr><tr><td>이메일</td><td>Connect User의 이메일 주소가 표시됩니다.<br>이메일 주소는 변경할 수 없습니다.</td></tr><tr><td>이름</td><td>Connect User의 이름이 표시됩니다.<br>이름은 변경할 수 없습니다.</td></tr><tr><td>상태</td><td>Connect User를 ‘유효’ 또는 ‘무효’로 설정할 수 있습니다.</td></tr><tr><td>사용 권한</td><td><p>사용 가능한 기능 접근 가능한 폴더에 관한 다음 정보가 표시됩니다.</p><ul><li>폴더<br>접근 가능한 폴더의 경로가 표시됩니다.</li><li>초대자<br>현재 선택된 Connect User를 초대한 사용자가 표시됩니다.</li><li>등록일<br>대상 폴더에 대한 접근이 유효해진 일시가 표시됩니다.</li><li>유효기간<br>대상 폴더에 접근할 수 있는 기간의 확인 및 변경이 가능합니다.</li><li>권한<br>대상 폴더에 설정된 접근 권한의 확인 및 변경이 가능합니다.</li><li>삭제<br>대상 폴더에 설정된 접근 권한을 해제할 수 있습니다.</li></ul></td></tr></tbody></table>

