---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_share/management_in_link
---

# 링크 수신 화면에서 미리보기, 다운로드, 업로드를 하는 방법

### 개요 <a href="#a03" id="a03"></a>

공유 링크의 수신자는 [\[Web\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/w_link_check) 또는 [\[Dirve\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/d_link_check)에 기재된 접근 권한 범위 내에서 파일을 조작할 수 있습니다. \
이 매뉴얼에서는 공유 링크 수신 화면에서 미리보기, 다운로드, 업로드 작업을 수행하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 공유 링크 수신 화면은, 사용 중인 기기나 애플리케이션 종류와 상관없이 반드시 Web 브라우저에서 표시됩니다. 각 애플리케이션 내부에서 표시하는 것은 불가능합니다.
* 링크 알림 메일의 발신자 정보에 포함되는 이름은, no-reply 메일에 회신할 수 있도록 설정되어 있는지 여부에 따라 달라집니다.
  * no-reply 메일에 회신할 수 있는 경우:\
    사용자 이름 no-reply@directcloud.jp
  * no-reply 메일에 회신할 수 없는 경우:\
    DirectCloud no-reply@directcloud.co.jp
* 비밀번호 입력 화면의 입력란은 `Ctrl+V` 붙여넣기와 우클릭 메뉴를 통한 붙여넣기에도 대응합니다.
* [\[Web\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/w_link_check) 또는 [\[Dirve\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/d_link_check)의 설정에 따라 비밀번호 옵션의 체크를 해제한 상태로 링크를 전송한 경우에는 비밀번호 입력 화면이 표시되지 않습니다.
* [파일을 다운로드하지 않고 미리 볼 수 있도록 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/file_preview)에서 “사용 안함”으로 설정한 경우, 해당 파일은 공유 링크 수신 화면에서 미리보기할 수 없습니다.
* 공유 링크 수신 화면에서 미리보기할 수 있는 파일의 확장자와 용량 제한은 [\[Web, Drive\] 파일을 다운로드하지 않고 미리보기하는 방법](https://help.directcloud.net/user_manual/file_management/wd_preview)을 참고하십시오.
* 링크 수신 화면에서 파일을 미리보기할 때 표시되는 일시는 파일의 갱신 일시이며, 이를 비표시로 변경할 수는 없습니다. 같은 파일명으로 덮어쓰기 저장을 하면, 링크 수신 화면에 표시되는 파일의 갱신 일시도 변경됩니다.
* 공유 링크 수신 화면에서는 폴더를 업로드할 수 없습니다.
* DirectCloud에는 DirectCloud-SHIELD IRM으로 암호화된 파일을 업로드할 수 없습니다.
* [폴더 용량 제한을 설정하는 방법](https://help.directcloud.net/admin_manual/folder/folder_capacity_limit)에서 제한된 용량을 초과하는 파일을 링크로 업로드할 수 없습니다.
* 공유 링크 수신 화면에서의 파일 업로드 최대 용량은 [\[Web\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/w_link_check) 또는 [\[Dirve\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/d_link_check)에 기재된 업로드 설정에 따라 달라집니다.
* 공유 링크 수신 화면에서 업로드한 파일과 동일한 이름의 파일이 업로드 대상 폴더에 이미 저장되어 있는 경우, [같은 이름의 파일 업로드 시 처리 기준 설정 방법](https://help.directcloud.net/admin_manual/upload/same_name_file)에서 어떤 설정을 하였는지와 관계없이 파일 이름 끝에 숫자가 붙어 별도의 파일로 업로드됩니다.
* 링크 생성 화면에서 업로드를 허용하도록 설정했더라도, 링크 생성 후 링크 대상 파일이 저장된 폴더를 이동하면 업로드가 불가능해지므로 공유 링크 수신 화면에는 업로드 버튼이 표시되지 않습니다.
* [업로드 가능한 파일의 크기를 제한하는 방법](https://help.directcloud.net/admin_manual/upload/limit_file_size)의 절차에서 파일 단위 용량 제한이 활성화되어 있는 경우, 링크로 업로드할 수 있는 파일의 용량 상한은 설정된 수치로 제한됩니다.
* 링크 업로드에서는 네트워크 장애 등으로 인해 일시 중지된 업로드를 재개하는 기능을 지원하지 않습니다.
* 링크 생성 화면에서 업로드를 허용하도록 설정한 경우, 업로드 진행 중에 업로드 대상 경로가 삭제되면 업로드가 실패합니다. 또한 업로드 대상 폴더가 이동되어, 이동한 위치의 상위 폴더 설정에 따라 접근 권한이 제거된 경우에도 업로드는 실패합니다.
* 공유 링크 수신 화면에서 파일을 미리보기할 때의 세션 시간은 20분입니다.
* 공유 링크로 전송된 폴더에 여러 개의 파일이 포함된 경우, 특정 파일만 미리보기를 할 수 없도록 설정하는 것은 불가능합니다.
*   링크 접근 횟수는 세션 단위로 계산되며, 그 횟수는 링크를 연 Web 브라우저에 쿠키로 저장됩니다.\
    따라서 한 사용자가 동일한 세션에서 10번 링크에 접근하더라도 접근 횟수는 1회로 계산됩니다.

    브라우저의 방문 기록을 삭제하거나, 브라우저를 연 후 24시간이 지나면 해당 세션은 종료됩니다.
* 전송한 링크를 열 때, 두 번째 이후에도 비밀번호를 입력하도록 설정하는 기능은 제공되지 않습니다.
* 링크 생성 화면에서 URL을 클릭해도 링크 수신 화면의 접근 횟수에는 포함되지 않습니다.\
  단, 다음의 경우는 접근 횟수에 포함됩니다.
  * Google Chrome 이외의 브라우저를 사용하여 별도의 탭에서 링크를 연 경우
  * 브라우저를 연 후 24시간이 지난 경우
*   링크 생성자가 아래의 어느 상황에 해당하는 경우, 링크에 접근한 수신자에게는 "이용이 제한되어 있습니다. 관리자에게 문의하십시오." 라는 오류 메시지가 표시되며, 해당 폴더 또는 파일에 접근할 수 없습니다.\
    설정이 원래 상태로 돌아가면 다시 링크 접근이 가능해집니다.

    * 링크 생성 후, 대상 폴더 또는 파일이 저장된 폴더에 대한 접근 권한이 삭제된 경우
    * 링크 생성 후, 관리자가 링크 생성 기능을 사용할 수 없도록 설정을 변경한 경우

    자세한 내용은 [특정 그룹이나 사용자에게 공유 링크 사용을 허용하지 않도록 설정하는 방법](https://help.directcloud.net/admin_manual/security_policy/link_restriction)과 [Guest의 링크 생성 가능 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/user/guest_link_permission)을 참고하십시오.

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**공유 링크 수신 화면 표시**
{% endhint %}

1. '○○님이 파일을 전송했습니다.'라고 하는 제목의 메일을 확인하고 '접속URL'에 있는 링크를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1470).png" alt=""><figcaption></figcaption></figure>

비밀번호가 설정된 링크 메일의 경우 비밀번호 입력 화면이 표시됩니다.\
비밀번호 입력 화면이 표시되지 않으면 3단계로 진행합니다.



2. 비밀번호를 보내는 방법에 따라 비밀번호를 입력합니다.

❶ 공유 링크의 비밀번호 송신 방법으로서 '비밀번호 별도 이메일로 발송'을 선택한 경우, 링크 메일과는 별도로 '\[  DirectCloud] 링크 비밀번호 안내'라는 제목의 메일이 도착합니다. 해당 이메일에 나열된 '비밀번호'를 입력하고 '확인' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1471).png" alt=""><figcaption></figcaption></figure>

❷ 공유 링크의 비밀번호 송신 방법으로 '비밀번호 동봉 발송'을 선택한 경우 링크 메일에 기재된 비밀번호를 입력하고 '확인'버튼을 클릭합니다.



3. 링크 수신 화면이 표시되면 링크 메일을 받은 이메일 주소를 입력하고 '확인' 버튼을 클릭합니다.\
   [링크를 수신할 때, 이메일 주소 입력을 통해 본인 확인을 진행하도록 설정하는 방법](https://help.directcloud.net/user_manual/file_share/wd_identity_verification)으로 이메일 주소를 입력하도록 설정하지 않았다면, 이 화면은 나타나지 않습니다.

<figure><img src="../../.gitbook/assets/image (188).png" alt="" width="563"><figcaption></figcaption></figure>



4. 공유 링크 수신 화면이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1052).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**공유 링크 수신 화면에서 미리보기**
{% endhint %}

1. 공유 링크 수신 화면에서 파일을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1053).png" alt=""><figcaption></figcaption></figure>

미리보기 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1054).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**공유 링크 수신 화면에서 다운로드**
{% endhint %}

1. 공유 링크 받기 화면에서 파일 왼쪽을 체크하고 '다운로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1055).png" alt=""><figcaption></figcaption></figure>

파일이 다운로드됩니다.



2. 다운로드한 파일을 열고 문제없는지 확인합니다.



{% hint style="warning" %}
**공유 링크 수신 화면에 파일 업로드**
{% endhint %}

1. 공유 링크 수신 화면에서 업로드 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1056).png" alt=""><figcaption></figcaption></figure>

업로드 화면이 표시됩니다.



2. '+ 추가' 버튼을 클릭하여 업로드할 파일을 선택하거나 회색 영역으로 파일을 드래그 앤 드롭합니다.

<figure><img src="../../.gitbook/assets/image (1057).png" alt=""><figcaption></figcaption></figure>

업로드할 파일이 설정됩니다.

<figure><img src="../../.gitbook/assets/image (1058).png" alt=""><figcaption></figcaption></figure>

3. 링크를 보낸 사람에게 메시지를 보내려면 메시지 텍스트 상자에 입력합니다.

<figure><img src="../../.gitbook/assets/image (1059).png" alt=""><figcaption></figcaption></figure>

4. 전송 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1060).png" alt=""><figcaption></figcaption></figure>

업로드 프로세스의 상태 화면이 표시됩니다.



5. '업로드가 완료되었습니다'라는 메시지가 표시되는지 확인하고 '확인' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1062).png" alt=""><figcaption></figcaption></figure>

파일이 업로드됩니다.



**\[알림 이메일 확인]**

파일이 업로드되면 "업로더" 이외의 접근 권한이 부여된 공유 폴더에 대한 접근 권한이 있는 모든 사용자에게 "Shared Box에 신규 파일이 업로드 되었습니다."라는 제목의 알림 메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (1063).png" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
**공유 링크 수신 화면의 표시 언어 변경**
{% endhint %}

1. 공유 링크 수신 화면의 오른쪽 상단에 표시되는 "English"를 클릭합니다.



2. 표시되는 언어 목록에서 변경할 언어를 선택합니다.

![](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001dAb\&feoid=00N2w00000JMb2T\&refid=0EMBB000000Rbvy)



3. 회사 이름, 보낸 사람 이름, 파일 이름 이외의 표시가 선택한 언어로 변경되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1065).png" alt=""><figcaption></figcaption></figure>
