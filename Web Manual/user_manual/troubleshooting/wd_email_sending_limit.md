---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/troubleshooting/wd_email_sending_limit
---

# \[Web, Drive] '발송 제한된 수신자 목록'에 등록되어 있어 메일을 전송할 수 없는 이메일 주소가 있는 경우의 대처 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, 아래의 절차에 따라 수신자에 이메일 주소를 추가하여 메일을 발송하려고 했을 때, '발송 제한된 수신자 목록'에 등록되어 있다고 표시되어 메일을 발송할 수 없었던 경우의 대처 방법에 대해 설명합니다.

* [\[Web, Drive\] 링크를 생성해 공유하는 방법](https://help.directcloud.net/user_manual/file_share/wd_link_share)
* [파일을 이메일에 첨부하여 전송하는 방법](https://help.directcloud.net/user_manual/file_share/attachment_mail)
* [\[Web, Drive\] 계정이 없는 상대로부터 파일을 받는 방법(업로드 요청 기능)](https://help.directcloud.net/user_manual/file_share/wd_file_request)
* [사용자 페이지에서 Guest를 초대하는 방법](https://help.directcloud.net/user_manual/file_share/invitaion_guest)
* [Connect User를 초대하는 방법](https://help.directcloud.net/user_manual/file_share/invitaion_connect_user)

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 페이지에서 수신처 제한이 활성화되어 있는 경우에만 '이메일 발송 제한' 화면이 표시됩니다.
* 공유 링크 및 파일첨부 메일발송에 워크플로우가 설정되어 있는 경우에도 '이메일 발송 제한' 화면이 표시됩니다.
* 이메일 주소가 DirectCloud 필터에 등록되어 있을 때 표시되는 '반송 이력 알림' 화면에서는, 비활성화된 이메일 주소는 해제되어 메일이 전송됩니다.\
  반면, '발송 제한된 수신자 목록' 화면에서는 제한된 이메일 주소는 제외된 상태로 메일이 전송됩니다.
* 관리 페이지의 '로그 현황' > '링크 이력' 메뉴에서 표시되는 '링크 이력 상세' 화면에는, 발송 제한된 수신자 목록에 대한 정보는 표시되지 않습니다.
* 입력한 수신처 이메일 주소가 모두 제한되어 있는 경우에는 '전송' 버튼을 클릭하더라도 메일이 전송되지 않으며, '수신처를 입력해 주세요.'라는 오류 메시지가 표시됩니다.
* '발송 제한된 수신자 목록'에 추가된 이메일 주소 및 도메인이 메일 서버의 필터에도 등록되어 있는 경우에는, '이메일 발송 제한' 화면만 표시되고 '반송 이력 알림' 화면은 표시되지 않게 됩니다.
* '발송 제한된 수신자 목록'과 메일 서버 필터에 각각 여러 개의 이메일 주소가 등록되어 있는 경우에는, 먼저 '이메일 발송 제한' 화면에 '발송 제한된 수신자 목록'에서 제한된 이메일 주소가 표시되고, 이후 '반송 이력 알림' 화면에 메일 서버 필터에서 제한된 이메일 주소가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에 표시될 때의 해결 방법**
{% endhint %}

'공유 링크', '파일첨부 메일발송', '업로드 요청', 'Guest 초대', 'Connect User 초대' 중 어느 하나의 기능에서 메일을 전송하려고 할 때 '이메일 발송 제한' 화면이 표시되는 경우에는, 입력한 이메일 주소로의 전송이 제한되어 있습니다.\
이 경우의 동작은 아래와 같습니다.

1. 보내기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (685).png" alt=""><figcaption></figcaption></figure>

&#x20;      제한된 이메일 주소는 제외된 상태로 메일이 전송됩니다.\
&#x20;      제한을 해제하고 싶은 경우에는 관리자에게 문의해 주시기 바랍니다.



{% hint style="warning" %}
**DirectCloud 드라이브에 표시될 때의 해결 방법**
{% endhint %}

'공유 링크', '업로드 요청' 중 어느 하나의 기능에서 메일을 전송하려고 할 때 '이메일 발송 제한' 화면이 표시되는 경우에는, 입력한 이메일 주소로의 전송이 제한되어 있습니다.\
이 경우의 동작은 아래와 같습니다.

1. 보내기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (686).png" alt=""><figcaption></figcaption></figure>

&#x20;      제한된 이메일 주소는 제외된 상태로 메일이 전송됩니다.\
&#x20;      제한을 해제하고 싶은 경우에는 관리자에게 문의해 주시기 바랍니다.
