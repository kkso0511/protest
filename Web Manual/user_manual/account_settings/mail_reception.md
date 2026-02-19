---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/account_settings/mail_reception
---

# 사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 다음과 같은 작업에 대한 알림 메일을 수신할지 여부를 사용자 페이지에서 설정하는 방법을 설명합니다.

* 신규 로그인 시 알림 이메일
* 코멘트 수신 시 발송되는 이메일
* 신규파일 업로드 알림 이메일
* 자동삭제 설정된 파일삭제 시 알림 이메일

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 사용자 페이지에서 알림 이메일 수신 여부를 설정할 수 있도록 하려면,\
  [사용자가 사용자 페이지에서 알림 메일 수신 여부를 결정할 수 있도록 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/user_email_setting)의 절차에 따라, ‘알림 이메일 수신 거부 권한’이 ‘사용’으로 설정되어 있어야 합니다.
* 이 매뉴얼의 절차로는 사용자 로그인, 파일 업로드, 파일에 코멘트 추가, 폴더 속성 자동 삭제 이외의 알림 이메일은 활성화 또는 비활성화할 수 없습니다.
* [사용자 정보를 변경하는 방법](https://help.directcloud.net/admin_manual/user/edit_user)에서 이메일 주소를 변경하면, 알림 이메일의 수신 주소도 함께 변경됩니다.
* 알림 이메일의 제목은 변경할 수 없습니다.
* 알림 이메일의 수신 대상을 특정 사용자로 지정할 수는 없습니다.
* 로그인 알림은 아래 조건을 모두 충족하는 경우에만 발송됩니다.
  * [사용자가 로그인했을 때 알림 메일이 발송 되도록 관리 페이지에서 설정하는 방법](https://help.directcloud.net/admin_manual/security_policy/login_notification)의 절차에 따라, ‘알림 이메일 발송’을 ‘사용’으로 설정
  * 이 매뉴얼의 절차에서 ‘알림 이메일’을 ‘수신’으로 설정
* 파일에 코멘트가 추가되었을 때의 알림 이메일은 아래 조건을 모두 충족하는 경우에만 발송됩니다.
  * [파일 코멘트 기능을 사용하는 방법](https://help.directcloud.net/admin_manual/detail_settings/enable_comment) 및 [특정 폴더에서 코멘트를 사용하도록 설정하는 방법](https://help.directcloud.net/admin_manual/folder/enable_comment)에 따라, 파일 코멘트 기능을 활성화
  * [파일에 코멘트가 추가되었을 때 알림 메일의 전송 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/comment_email_notification)에서, 이메일 알림을 ‘사용’으로 설정
  * [\[Web, Drive\] 파일 코멘트를 추가하는 방법](https://help.directcloud.net/user_manual/file_management/wd_comment)에서 ‘이메일 알림’에 체크
  * 이 매뉴얼의 절차에서 ‘알림 이메일’을 ‘수신’으로 설정
* 파일이 업로드되었을 때의 알림 이메일은 아래 조건을 모두 충족하는 경우에만 발송됩니다.
  * [관리자 페이지에서 폴더를 생성하는 방법](https://help.directcloud.net/admin_manual/folder/create_folder) 또는 [관리자 페이지에서 폴더 이름을 변경하는 방법](https://help.directcloud.net/admin_manual/folder/rename_folder)에서, ‘알림 설정’을 ‘사용’으로 설정
  * 이 매뉴얼의 절차에서 ‘알림 이메일’을 ‘수신’으로 설정
* 폴더 속성 설정에 따른 자동 삭제 알림은 아래 조건을 모두 충족하는 경우에만 발송됩니다.
  * [Shared Box의 폴더, 파일이 자동으로 삭제되도록 설정하는 방법](https://help.directcloud.net/admin_manual/folder/sharedbox_auto_delete)에서, ‘삭제 후 확인 이메일 발송’에 체크
  * [파일에 유효기간을 설정하는 방법](https://help.directcloud.net/user_manual/file_management/expiration_date)에서 ‘이메일을 받지 않음’의 체크를 해제
  * 이 매뉴얼의 절차에서 ‘알림 이메일’을 ‘수신’으로 설정
* 위 알림 조건을 충족했음에도 알림 이메일을 수신하지 못하는 경우에는,\
  알림 조건을 충족했지만 알림 이메일이 도착하지 않는 경우의 대처 방법을 참고하시기 바랍니다.
* 위 알림 조건에 해당하지 않는데도 알림 이메일을 수신한 경우에는, 아래 사항을 확인해 주세요.
  * 동일한 이메일 주소로 등록된 사용자 또는 Guest가 이메일 알림을 ‘수신’으로 설정해 두었는지
  * 해당 이메일 주소가 포함된 그룹 메일로 등록된 사용자 또는 Guest가 이메일 알림을 ‘수신’으로 설정해 두었는지

### 절차 <a href="#a05" id="a05"></a>

1. 다음 중 한 가지 방법으로 ‘설정’ 화면을 표시합니다.

❶  사용자 이름 클릭

<figure><img src="../../.gitbook/assets/image (664).png" alt=""><figcaption></figcaption></figure>

❷  설정 버튼을 클릭

<figure><img src="../../.gitbook/assets/image (663).png" alt=""><figcaption></figcaption></figure>



2. '이메일 알림'을 수신으로 설정합니다.

<figure><img src="../../.gitbook/assets/image (662).png" alt=""><figcaption></figcaption></figure>

설정은 즉시 저장됩니다.
