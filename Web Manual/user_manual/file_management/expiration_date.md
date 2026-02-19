---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_management/expiration_date
---

# 파일에 유효 기간을 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, 파일에 유효 기간을 설정하여 일정 기간이 지나면 파일이 자동으로 삭제되도록 구성하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼 에서는 Shared Box와 Connect 폴더에서의 조작 방법을 설명하고 있지만, My Box와 DLP 폴더도 동일한 절차로 이용하실 수 있습니다.
* 아래의 폴더에서는 파일의 유효 기간을 설정할 수 없습니다.
  * Connect 폴더
  * Warm Storage의 폴더
* 파일의 유효 기간을 설정하려면 <마스터>, <전체권한>의 접근 권한이 부여되어 있어야 합니다.\
  자세한 내용은 접근 권한의 종류와 Web 브라우저에서 가능한 작업을 참조해주시기 바랍니다.
* Guest도 파일의 유효 기간을 설정할 수 있습니다.
* Connect User는 파일의 유효 기간을 설정할 수 없습니다.
* 이 매뉴얼의 절차로는 폴더에 유효 기간을 설정할 수 없습니다.\
  그러나 [Shared Box의 폴더, 파일이 자동으로 삭제되도록 설정하는 방법](https://help.directcloud.net/admin_manual/folder/sharedbox_auto_delete)을 사용하면 폴더가 자동 삭제되도록 설정할 수 있습니다.
* 파일 유효 기간에 따른 자동 삭제는 설정한 다음 날부터 계산되며, 계산일을 포함해 지정한 기간이 지난 후 다음 날 새벽 2시 0분 0초에 실행됩니다.
* 자동 삭제 실행 시간은 변경할 수 없습니다.
* 파일 유효 기간의 기본값(30일 후)은 변경할 수 없습니다.
*   한 번 파일 기간을 설정하면 해당 파일이 자동 삭제될 때까지 남은 일수를 변경할 수 없습니다.

    파일의 유효 기간을 해제하려면, 이 매뉴얼의 파일의 유효 기간을 해제하는 절차를 따라 설정을 해제하신 후, 다시 파일에 유효 기간을 설정하는 절차를 진행해주시기 바랍니다.
* 파일의 유효 기간에 의해 삭제된 파일은 관리자 휴지통으로 이동합니다.\
  자세한 내용은 [회사 휴지통으로 이동 한 폴더, 파일을 확인하는 방법](https://help.directcloud.net/admin_manual/storage/company_trash_check)을 참조해주시기 바랍니다.
* 파일의 유효 기간을 설정한 이력은 관리 페이지의 '로그현황' > '파일 기한 설정 현황' 목록 메뉴에서 확인하실 수 있습니다.\
  파일의 유효 기간을 해제한 이력은 기록되지 않습니다.
* 유효 기간으로 인해 삭제된 파일의 이력은 관리 페이지의 '로그 현황'> '파일 이용 내역'에서 확인할 수 있습니다.
* [사용자 페이지에서 알림 메일의 수신 여부를 설정하는 방법](https://help.directcloud.net/user_manual/account_settings/mail_reception)을 통해, 파일 기한으로 인해 파일이 삭제되었을 때 알림 메일을 받도록 설정할 수는 없습니다.
* DirectCloud-CONNECT를 이용할 수 있는 경우, 사용자 페이지에 Connect 메뉴가 표시됩니다.
* DirectCloud-SHIELD DLP를 이용 중인 경우, 사용자 페이지에 DLP 메뉴가 표시됩니다.
* Warm Storage를 계약한 경우, 사용자 페이지에 Warm Storage 메뉴가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**'파일 기한' 화면 표시**
{% endhint %}

**\[Shared Box에 표시]**

1. 파일 기한일을 설정하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1356).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나를 사용하여 파일 기한일을 설정합니다.

❶  파일 기한일을 설정하고자 하는 파일을 체크하고 상단의 '파일 기한' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1357).png" alt=""><figcaption></figcaption></figure>

❷  파일 기한일을 설정하려는 파일을 마우스 오른쪽 버튼으로 클릭하고 "파일 기기한"을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1358).png" alt=""><figcaption></figcaption></figure>

❸  파일 기한일을 설정하고자 하는 파일의 오른쪽에 있는

<figure><img src="../../.gitbook/assets/image (1359).png" alt=""><figcaption></figcaption></figure>

'파일 기한' 메뉴가화면이 표시됩니다.



**\[파일에 만료 날짜 설정]**

1. 파일 기한 화면에서 파일이 자동으로 삭제되기까지의 일수로 1\~365 사이의 숫자를 입력합니다.

<figure><img src="../../.gitbook/assets/image (1360).png" alt=""><figcaption></figcaption></figure>



2. 파일이 삭제될 때 알림 메일을 받지 않으려면 '이메일 수신 안함'에 체크합니다.

<figure><img src="../../.gitbook/assets/image (1361).png" alt=""><figcaption></figcaption></figure>



3. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1362).png" alt=""><figcaption></figcaption></figure>



4. 설정된 파일 기한을 확인하고 ✕ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1363).png" alt=""><figcaption></figcaption></figure>



**\[파일 기한 설정 해제]**

1. 파일 기한을 해제고자 하는 파일의 '파일 기한' 화면을 표시합니다.



2. '설정해제' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1364).png" alt=""><figcaption></figcaption></figure>



3. '설정일'과 '삭제 예정일' 표시가 사라졌는지 확인하고 '✕' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1365).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**파일 기한으로 삭제된 경우의 알림 메일 확인**
{% endhint %}

'파일 기한' 화면에서 '이메일 수신안함'을 체크하지 않고 설정한 경우, '파일 유효기간 경과에 따른 파일삭제 알림.'이라는 제목의 알림 메일이 도착합니다.

<figure><img src="../../.gitbook/assets/image (1815).png" alt=""><figcaption></figcaption></figure>
