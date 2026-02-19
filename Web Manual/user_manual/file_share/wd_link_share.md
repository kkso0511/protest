---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_share/wd_link_share
---

# \[Web, Drive] 링크를 생성해 공유하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 폴더와 파일에 접근할 수 있는 링크를 생성하고, 수신자를 지정하여 전달하는 기본적인 방법을 설명합니다.\
링크 생성 화면의 구성과 설정 항목에 대한 내용은 [\[Web\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/w_link_check) 또는 [\[Dirve\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/d_link_check)을 참고해주시기 바랍니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 페이지의  '보안정책'->'사용권한' 에서 'File Link'에 체크가 되어 있는 권한 세트가 그룹 또는 사용자에게 부여되어 있어야 합니다.
* DLP 폴더에서 링크 생성 화면을 표시하려면 DLP 설정에서 사용자에게 링크 생성을 허용하도록 설정하는 방법의 절차에 따라 링크 설정의 사용함에 체크되어 있어야 합니다.
* 링크 생성 화면을 표시하려면, [특정 폴더에서 링크 생성 기능을 활성화하는 방법](https://help.directcloud.net/admin_manual/folder/enable_link_creation)의 절차에 따라 아래와 같이 설정해야 합니다.
  * Shared Box, DLP: '폴더 옵션' 설정에서 '링크'의 '사용'에 체크
* Connect 폴더와 Warm Storage 폴더에서는 링크 생성 화면을 표시할 수 없습니다.
* 폴더 및 파일의 Shared Box 링크를 생성하려면 <마스터>, <전체권한>, <편집자>의 접근 권한이 부여되어 있어야 합니다.
* Guest 기능 제한에서 Guest가 링크를 생성하지 못하도록 설정되어 있는 경우 아래의 버튼과 메뉴는 표시되지 않습니다. 자세한 내용은 [Guest의 링크 생성 가능 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/user/guest_link_permission)을 참고해주시기 바랍니다.
  * Web 브라우저\
    사용자 페이지의 링크 생성 메뉴와 링크 생성 버튼
  * DirectCloud 드라이브\
    우클릭 메뉴의 'DirectCloud-Drive' > '링크 생성'
* 사용자 로그인 페이지의 메인 도메인을 설정하는 방법의 절차에서 링크 URL의 도메인을 설정하면, 생성되는 링크 URL의 메인 도메인도 함께 변경됩니다.
* 사용자 로그인 페이지의 메인 도메인을 변경하더라도, 변경 이전에 생성된 Shared Box 링크에는 계속 접근할 수 있습니다.
* 수신자, Cc/Bcc, 제목, 내용을 입력한 뒤 링크 생성 화면 오른쪽 상단의 X 버튼 또는 취소 버튼을 클릭하면 설정 내용이 일시적으로 저장됩니다. 이후 동일한 폴더나 파일에서 링크 생성을 다시 시작하고 표시되는 확인 화면에서 확인 버튼을 클릭하면 일시 저장된 설정 내용을 불러와서 표시할 수 있습니다.
* 링크 생성 화면의 발신자에 표시되는 이메일 주소는 no-reply 메일에 회신할 수 있도록 설정되어 있는지 여부에 따라 달라집니다.
  * no-reply 메일에 회신할 수 있는 경우:\
    사용자 이름no-reply@directcloud.jp
  * no-reply 메일에 회신할 수 없는 경우:\
    DirectCloudno-reply@directcloud.co.jp
*   링크의 접근 횟수는 세션 단위로 계산되며, 해당 횟수는 링크를 연 Web 브라우저에 쿠키로 저장됩니다.\
    따라서 동일한 사용자가 같은 세션에서 링크에 10회 접근하더라도 접근 횟수는 1회로 처리됩니다.

    브라우저의 방문 기록을 삭제하거나 브라우저를 연 뒤 24시간이 지나면 해당 세션은 종료됩니다.
* 전달한 링크를 열 때 두 번째 이후에도 비밀번호를 다시 입력하도록 설정할 수는 없습니다.
* 링크 생성 화면에서 URL을 클릭해도 링크 수신 화면의 접근 횟수에는 추가되지 않습니다.\
  단, 아래의 경우에는 접근 횟수가 추가됩니다.
  * Google Chrome 이외의 브라우저에서 다른 탭으로 링크를 연 경우
  * 브라우저를 연 뒤 24시간이 지난 경우
* 링크 생성 화면에 표시되는 언어는 [사용자 페이지의 표시 언어를 변경하는 방법](https://help.directcloud.net/user_manual/account_settings/change_language)으로 바꿀 수 있습니다.
* 링크를 생성한 후 대상 폴더 또는 파일이 저장된 폴더에 대한 접근 권한이 제거된 경우, 링크 대상의 폴더와 파일에 접근할 수 없습니다.\
  링크를 생성한 사용자의 접근 권한이 제거되면 링크 수신자 또한 해당 폴더 및 파일에 접근할 수 없습니다.
* 링크 수신 화면에서 파일을 미리보기 할 때 표시되는 날짜와 시간은 파일의 업데이트 시각입니다. 이 날짜와 시간은 비표시로 설정할 수 없습니다.같은 파일명으로 덮어쓰기 저장하면 링크 수신 화면의 파일 업데이트 시각도 변경됩니다.
* [폴더 용량 제한을 설정](https://help.directcloud.net/admin_manual/folder/folder_capacity_limit)한 경우, 제한된 용량을 초과하는 파일은 링크를 통해 업로드할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 공유 링크 생성 및 전송**
{% endhint %}

1. [\[Web\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/w_link_check)의 순서로 공유 링크를 생성하고 싶은 폴더 또는 파일의 링크 생성 화면을 표시합니다.



2. '받는 사람' 입력란에 링크를 보내고자 하는 이메일 주소를 입력합니다.\
   입력란 외의 영역을 클릭하면 입력한 이메일 주소가 반영됩니다.\
   [회사·개인 주소록을 활성화하는 방법](https://help.directcloud.net/admin_manual/detail_settings/enable_addressbook)의 절차에 따라 주소록이 활성화되어 있는 경우, 오른쪽에 표시되는 아이콘을 클릭하여 주소록에서 수신자 이메일 주소를 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1289).png" alt=""><figcaption></figcaption></figure>



3. 필요한 경우 제목과 내용을 입력합니다.

<figure><img src="../../.gitbook/assets/image (1290).png" alt=""><figcaption></figcaption></figure>



4. 전송되는 이메일의 내용을 확인하려면 미리보기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1291).png" alt=""><figcaption></figcaption></figure>

메일 내용이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1292).png" alt=""><figcaption></figcaption></figure>



5. 설정한 내용으로 링크를 보낼 수 있는 경우에는 '보내기' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1293).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 공유 링크 생성 및 전송**
{% endhint %}

1. [\[Dirve\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/d_link_check)의 순서로 공유 링크를 만들려는 폴더 또는 파일의 "링크 만들기"화면을 표시합니다.



2. '받는 사람' 입력란에 링크를 보내고자 하는 이메일 주소를 입력합니다.\
   입력란 외의 영역을 클릭하면 입력한 이메일 주소가 반영됩니다.\
   [회사·개인 주소록을 활성화하는 방법](https://help.directcloud.net/admin_manual/detail_settings/enable_addressbook)의 절차에 따라 주소록이 활성화되어 있는 경우, 오른쪽에 표시되는 아이콘을 클릭하여 주소록에서 수신자 이메일 주소를 선택할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1294).png" alt=""><figcaption></figcaption></figure>



3. 필요한 경우 제목과 내용을 입력합니다.

<figure><img src="../../.gitbook/assets/image (1295).png" alt=""><figcaption></figcaption></figure>



4. 전송되는 이메일의 내용을 확인하려면 '미리보기' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1291).png" alt=""><figcaption></figcaption></figure>

메일 내용이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1296).png" alt=""><figcaption></figcaption></figure>



5. 설정한 내용으로 링크를 보낼 수 있는 경우에는 '보내기' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1297).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**공유 링크 이메일 확인**
{% endhint %}

'링크 생성' 화면에서 만든 링크를 보내면 다음과 같은 이메일이 수신인에게 전송됩니다.

<figure><img src="../../.gitbook/assets/image (1298).png" alt=""><figcaption></figcaption></figure>
