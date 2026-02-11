---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-6/undefined-5
---

# 사용자가 사용자 페이지에서 알림 메일 수신 여부를 결정할 수 있도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 다음 작업이 실행될 때 사용자에게 알림 메일이 전송됩니다.\
각 작업에서 사용자가 알림 메일을 받을지 여부는 사용자 페이지에서 알림 메일을 받을지 여부를 설정하는 방법의 절차에 따라 설정할 수 있습니다.

・사용자 로그인\
・파일 업로드\
・파일에 코멘트 추가\
・폴더 속성 설정에 따른 자동 삭제

이 매뉴얼에서는 사용자가 알림 메일을 받을지 여부를 설정할 수 있는 권한을 부여하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* 이 매뉴얼의 절차에서는 사용자의 로그인, 파일 업로드, 파일에 코멘트를 추가하는 기능, 폴더 속성 설정에 따른 자동 삭제 외의 알림 메일을 활성화하거나 비활성화할 수 없습니다.
* [사용자 정보를 변경하는 방법](https://help.directcloud.net/admin_manual/undefined-3/undefined-1)의 절차에서 메일 주소를 변경하면 알림 메일의 수신처도 함께 변경됩니다.
* 알림 메일의 제목은 변경할 수 없습니다.
* 알림 메일의 수신자를 개별적으로 설정할 수 없습니다.
* 로그인 알림은 다음 조건을 모두 만족하는 경우에 전송됩니다
  * [사용자가 로그인했을 때 알림 메일이 발송 되도록 관리 페이지에서 설정하는 방법](https://help.directcloud.net/admin_manual/images-and-media/undefined-7)에서 알림 메일 전송을 사용함으로 설정한 경우
  * [사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법](https://help.directcloud.net/user_manual/undefined-13/undefined-3)에서 알림 메일을 수신함으로 설정한 경우
* 파일에 코멘트를 추가했을 때 발송되는 알림 메일은 다음 조건을 모두 충족하는 경우에 전송됩니다.
  * [파일 코멘트 기능을 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-6/undefined)에서 파일 코멘트 기능을 활성화로 설정할 것
  * [파일에 코멘트가 추가되었을 때 알림 메일의 전송 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/undefined-1)에서, 메일 알림을 '사용'으로 설정
  * [\[Web, Drive\] 파일 코멘트를 추가하는 방법](https://help.directcloud.net/user_manual/undefined-3/web-drive-1) 에서, '메일 알림'에 체크
  * [사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법](https://help.directcloud.net/user_manual/undefined-13/undefined-3)에서 알림 메일을 수신함으로 설정한 경우
* 파일이 업로드되었을 때의 알림 메일은 다음 조건을 모두 충족하는 경우에 전송됩니다.
  * [관리자 페이지에서 폴더를 생성하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined) 또는 [관리자 페이지에서 폴더 이름을 변경하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-1)에서 알림 설정을 사용함으로 설정할 것
  * [사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법](https://help.directcloud.net/user_manual/undefined-13/undefined-3)에서 알림 메일을 받기로 설정할 것
* 폴더 속성 설정에 따른 자동 삭제 알림 메일은 아래 조건을 모두 충족할 경우에 전송됩니다.
  * [Shared Box의 폴더, 파일이 자동으로 삭제되도록 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-4/shared-box-3)에서 삭제 후 확인 메일 송신에 체크함
  * [파일에 유효 기간을 설정하는 방법](https://help.directcloud.net/user_manual/undefined-3/undefined-2)에서 메일을 받지 않음의 체크를 해제함
  * [사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법](https://help.directcloud.net/user_manual/undefined-13/undefined-3)에서 알림 메일을 수신함으로 설정함
* [링크 수신 화면에서 미리보기, 다운로드, 업로드를 하는 방법](https://help.directcloud.net/user_manual/undefined-4/undefined)에 따라 공유 링크로 파일을 업로드하는 경우, 일반 파일 업로드와 동일한 알림 메일이 전송됩니다.
* 업로드 요청에 파일을 업로드한 경우에는 일반 파일 업로드와 동일한 알림 메일이 전송됩니다. 여기에 더해, [업로드 요청 폴더에 파일을 업로드하는 방법](https://help.directcloud.net/user_manual/undefined-4/undefined-1)에 따라 파일을 업로드한 사용자와 업로드를 요청한 사용자에게 알림 메일이 전송됩니다.
* 위의 알림 조건에 해당하는 경우라도 <업로더> 접근 권한이 부여된 사용자에게는 알림 메일이 전송되지 않습니다.

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**알림 메일 수신 거부 권한 설정**
{% endhint %}

1. '공유 설정' > '세부 기능 설정' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1997).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 '이메일 수신거부 선택권 설정'에서 '이메일 수신거부 선택권 제공'을 사용으로 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1998).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자 페이지에서 알림 이메일 설정 확인**
{% endhint %}

1. 사용자 페이지에서 사용자 프로필의 설정 화면을 클릭하면 '이메일 알림'설정이 보이며 알림 메일을 받을지 여부를 선택할 수 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1999).png" alt=""><figcaption></figcaption></figure>
