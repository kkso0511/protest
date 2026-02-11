---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-6/undefined-1
---

# 파일에 코멘트가 추가되었을 때 알림 메일의 전송 여부를 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 파일에 코멘트가 추가되었을 때 알림 메일이 전송되도록 설정하는 방법을 설명합니다. 또한, 기본으로 어떤 사용자에게 알림 메일을 보낼지 설정하는 방법도 함께 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* 메일 알림은 기본으로 사용함으로 설정되어 있습니다.
* 이 매뉴얼의 설정은 [파일 코멘트 기능을 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-6/undefined)에서 코멘트 기능을 사용함으로 설정한 경우에 표시됩니다.
* 파일 코멘트 기능은 PC Agent에서는 사용할 수 없습니다.
* 접근 권한 레벨이 업로더인 사용자는 파일 코멘트 기능을 사용할 수 없습니다.
* 아래의 모든 조건을 만족하는 경우, 파일에 코멘트가 추가되었을 때 알림 메일이 전송됩니다.
  * 이 매뉴얼의 절차에 따라 파일 코멘트 기능이 활성화되어 있을 것
  * [파일에 코멘트가 추가되었을 때 알림 메일의 전송 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/undefined-1)에서, 메일 알림을 '사용'으로 설정
  * [사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법](https://help.directcloud.net/user_manual/undefined-13/undefined-3)에서, 사용자 페이지의 알림 설정을 '수신'으로 설정
  * [\[Web, Drive\] 파일 코멘트를 추가하는 방법](https://help.directcloud.net/user_manual/undefined-3/web-drive-1)에서, 코멘트 입력란 왼쪽 하단에 있는 '메일 알림'에 체크
* 알림 조건을 모두 충족하더라도 <업로더> 접근 권한이 부여된 사용자에게는 알림이 전송되지 않습니다.

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**코멘트 알림 메일 사용**
{% endhint %}

1. '공유 설정' > '코멘트 설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1986).png" alt=""><figcaption></figcaption></figure>



2. '이메일로 코멘트 알림' 설정에서 '공유사용자에게 이메일 알림'을 사용을 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2326).png" alt=""><figcaption></figcaption></figure>

3. 알림 메일 수신 대상에서 기본으로 어떤 사용자에게 알림 메일을 보낼지 선택한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2327).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="189.20001220703125">항목</th><th>설명</th></tr></thead><tbody><tr><td>전체</td><td>접근 권한 레벨이 업로더가 아닌 모든 사용자에게 알림 메일이 전송됩니다.</td></tr><tr><td>To 대상</td><td>To 버튼을 클릭하여 추가한 사용자에게만 알림 메일이 전송됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**파일 코멘트 알림 이메일 확인**
{% endhint %}

파일 코멘트 알림이 활성화된 경우 파일 코멘트가 추가되면 "○○ 님이 코멘트를 남겼습니다."라는 제목의 알림 메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (1988).png" alt=""><figcaption></figcaption></figure>
