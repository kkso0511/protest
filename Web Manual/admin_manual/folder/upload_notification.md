---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/folder/upload_notification
---

# 특정 폴더에서 업로드 알림 기능을 사용하도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 관리 페이지에서 폴더를 선택하고 폴더 속성에서 사용자가 파일을 업로드했을 때 알림 메일을 보내도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼 에서는 환경 설정 메뉴의 Shared Box 및 Connect 관리 메뉴의 설정 방법을 설명하고 있으며, DLP 관리와 문서 관리 메뉴도 동일한 절차로 설정하실 수 있습니다.
* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* 초기 상태에서는 메일 알림이 사용함(5분마다 전송)으로 설정되어 있습니다.
* 메일 알림은 최상위 계층의 폴더에 설정하며, 설정한 내용은 하위 폴더에 그대로 적용됩니다.
* [관리자 페이지에서 폴더를 생성하는 방법](https://help.directcloud.net/admin_manual/folder/create_folder)의 알림 설정에서 지정한 내용이 반영됩니다.
* 메일 알림은 [사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법](https://help.directcloud.net/user_manual/account_settings/mail_reception)에서, 사용자 페이지의 알림 설정을 수신함으로 지정한 경우에만 유효합니다.
* 사용자 페이지의 알림 설정을 수신함으로 지정하더라도, 이 매뉴얼의 절차에서 알림을 사용하지 않음으로 설정한 경우에는 알림 메일이 전송되지 않습니다.
* 메일 알림을 사용함으로 설정하더라도 <업로더> 접근 권한이 부여된 사용자에게는 알림 메일이 전송되지 않습니다.
* 여러 개의 파일이 동시에 업로드된 경우에도 한 통의 알림 메일로 묶어서 전송됩니다.
* DirectCloud-SHIELD DLP를 계약한 경우, 관리 페이지에 DLP 관리 메뉴가 표시됩니다.
* DirectCloud-CONNECT를 이용할 수 있는 경우, 관리 페이지에 Connect 관리 메뉴가 표시됩니다.
* Warm Storage를 이용할 수 있다면, 관리 페이지에 Warm Storage 관리 메뉴가 표시됩니다.
* Cold Storage를 계약하고 있는 경우, 관리 페이지에 Cold Storage 관리 메뉴가 표시됩니다.
* Warm Storage와 Cold Storage에서는 업로드 시 알림 메일이 전송되지 않기 때문에, Warm Storage 관리 및 Cold Storage 관리 메뉴에서 폴더를 선택하더라도 폴더 속성에 메일 알림은 표시되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Shared Box 업로드 알림 사용**
{% endhint %}

1. '공유 설정' > 'Shared Box 관리' 메뉴를 선택하고 업로드 알림을 사용하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1960).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 폴더 속성 설정에서 '이메일 통지'의 '수정' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1961).png" alt=""><figcaption></figcaption></figure>



3. 이메일 통지에서 사용을 선택하고 알림 이메일을 보낼 간격을 선택한 다음 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1962).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**업로드 알림 이메일 확인**
{% endhint %}

메일 알림 설정이 활성화된 폴더에 파일이 업로드되면, 해당 폴더에 대한 액세스 권한이 있는 모든 사용자에게 "Shared Box에 신규 파일이 업로드 되었습니다." 라는 제목의 메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (335).png" alt="" width="563"><figcaption></figcaption></figure>
