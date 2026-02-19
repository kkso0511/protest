---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/custom_settings/gmail_email
---

# DirectCloud에서 발송하는 메일 주소를 Gmail로 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

공유 링크나 첨부 파일을 전송할 때는 기본적으로 \<no-reply@directcloud.jp>라는 메일 주소로 DirectCloud의 메일 서버에서 발송됩니다.\
이 매뉴얼에서는 송신 메일 서버 설정에서 본인의 Gmail 주소를 사용하여 DirectCloud에서 메일을 보내는 방법을 설명합니다.\
Gmail의 경우 OAuth를 이용해 연동하므로 사용자 ID·메일 주소·비밀번호를 입력할 필요가 없습니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정' 메뉴를 사용할 수 있습니다.
* 아래 기능에서 메일을 보낼 때 발신 메일 주소를 변경할 수 있습니다.
  * 공유 링크
  * 파일첨부 메일 발송
  * Guest 초대
  * Connect User 초대
  * 업로드 요청
* 메일의 발신 주소를 Gmail로 변경하는 경우, 한 번에 설정할 수 있는 수신자 메일 주소의 최대 개수는 무제한입니다. 따라서 수신자 수 제한 항목은 표시되지 않습니다.
* 기본 발신 메일 주소에서 자체 메일 주소로 변경하면 아래 기능을 사용할 수 있습니다.
  * 11명 이상의 수신자에게 전송
  * 반송 메일 수신
* 발신 메일 서버는 일괄 등록할 수 없습니다.
* 메일 서버에서 IP 주소 제한을 설정하고 있는 경우 54.64.42.47에서의 접근을 허용해야 합니다.
* 기본 발신 메일 주소는 기본으로 사용함으로 설정되어 있습니다.
* 발신 메일 서버 설정이 표시되지 않는 경우, 관리자 페이지의 표시 언어를 일본어 또는 영어로 설정한 상태에서 web 브라우저의 자동 번역 기능이 작동하고 있을 가능성이 있습니다.\
  이 경우 브라우저의 자동 번역 기능을 비활성화하고 캐시를 모두 삭제한 뒤 다시 표시해주세요.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**발신 메일 서버 설정**
{% endhint %}

1. '공유 설정' > '맞춤형 설정' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (452).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 '이메일 발신서버' 설정에서 보내는 서버 정보의 방식을 Gmail로로 선택합니다.

<figure><img src="../../.gitbook/assets/image (453).png" alt=""><figcaption></figcaption></figure>



3. 디폴트 발송 이메일 주소인 no-reply@directcloud.net 를 사용할 수 있는지 여부를 선택하고 저장 버튼을 클릭합니다. '사용 안함'을 선택하면 사용자는 이메일 작성 화면에서 이메일 주소를 설정해야 합니다.

<figure><img src="../../.gitbook/assets/image (454).png" alt=""><figcaption></figcaption></figure>



4. 보내는 메일 서버 설정의 사용을 선택합니다. 설정은 즉시 저장됩니다.

<figure><img src="../../.gitbook/assets/image (456).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Web 브라우저 또는 DirectCloud 드라이브에서 보낸사람 메일 주소를 등록하기**
{% endhint %}

1.  사용자 페이지에서 [\[Web, Drive\] 링크를 생성해 공유하는 방법](https://help.directcloud.net/user_manual/file_share/wd_link_share), [파일을 이메일에 첨부하여 전송하는 방법](https://help.directcloud.net/user_manual/file_share/attachment_mail)

    , [사용자 페이지에서 Guest를 초대하는 방법](https://help.directcloud.net/user_manual/file_share/invitaion_guest), [Connect User를 초대하는 방법](https://help.directcloud.net/user_manual/file_share/invitaion_connect_user), [업로드 요청 폴더에 파일을 업로드하는 방법](https://help.directcloud.net/user_manual/file_share/upload_to_file_request), 첨부 파일 전송, Guest 초대, 업로드 요청 화면 중 하나를 표시합니다.



2. 아래 방법 중 하나로 발신 메일 주소를 등록하는 화면을 표시합니다.

❶ '이메일 주소를 추가해 주세요.' 라고 표시되는 경우는 아래 두 조건을 모두 충족할 때입니다. \
&#x20;      이 경우 '발신 메일 주소를 등록해 주세요.' 를 클릭합니다.\
\
・관리자 페이지의 발신 메일 서버 설정에서 기본 발신 메일 주소가 사용하지 않음으로 설정되어 있음\
・메일 작성 화면의 발신 메일 주소 항목에 메일 주소가 등록되어 있지 않음

<figure><img src="../../.gitbook/assets/image (2321).png" alt="" width="421"><figcaption></figcaption></figure>



❷ 보낸사람 항목의 톱니바퀴 버튼을 클릭합니다. '보낸사람' 이메일 주소가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2322).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. '이메일 주소 추가'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2324).png" alt=""><figcaption></figcaption></figure>



4. 메일 주소 항목에서 'Gmail로 로그인'을 클릭합니다. Gmail 계정 선택 화면이 표시됩니다.

{% hint style="info" %}
**NOTE**\
이름 항목에 입력한 문자는 링크, 업로드 요청, 첨부 파일 전송, Guest 초대, Connect User 초대의 알림 메일의 수신자, 제목, 본문에서 DirectCloud의 사용자명 대신 표시됩니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (303).png" alt="" width="413"><figcaption></figcaption></figure>

&#x20;    &#x20;

5. 메일 전송에 사용할 계정을 입력 혹은 클릭합니다.

<figure><img src="../../.gitbook/assets/image (304).png" alt=""><figcaption></figcaption></figure>



6. 확인 화면에서 체크박스에 체크를 하고 '계속' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (305).png" alt=""><figcaption></figcaption></figure>

7. 필요에 따라 서명에서 추가를 선택하고, 메일 본문의 하단에 추가할 텍스트를 입력합니다.

<figure><img src="../../.gitbook/assets/image (306).png" alt=""><figcaption></figcaption></figure>



8. 설정한 메일 주소를 기본 메일 주소로 사용하려면 기본 메일 주소로 설정에 체크한 뒤 확인 버튼을 클릭합니다.\
   다른 발신 메일 주소를 지정할 수 없는 경우에는 이 체크를 해제할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (307).png" alt=""><figcaption></figcaption></figure>



9. Gmail에서 테스트 메일이 정상적으로 전송되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>



10. 이메일 주소가 "보낸 사람"에 추가되었는지 확인합니다.



{% hint style="warning" %}
**모바일에서 보낸사람 메일 주소를 등록하기**
{% endhint %}

1. 사용자 페이지에서 [\[Mobile\] 링크를 생성해 공유하는 방법](https://help.directcloud.net/user_manual/file_share/m_link_share), [\[Mobile\] 계정이 없는 상대로부터 파일을 받는 방법(업로드 요청 기능)](https://help.directcloud.net/user_manual/file_share/m_file_request)에 따라 공유 링크 또는 업로드 요청 화면 중 하나를 표시합니다.



2. 아래 방법 중 하나로 보낸사람 메일 주소를 등록하는 화면을 표시합니다.

❶ '이메일 주소가 필요합니다.' 라고 표시되는 경우는 아래 두 조건을 모두 충족할 때입니다. \
&#x20;     이 경우 '메일 주소를 등록해 주세요.' 를 탭합니다.

・관리자 페이지의 송신 메일 서버 설정에서 기본 발신 메일 주소가 사용하지 않음으로 설정되어 있음\
・메일 작성 화면의 발신 메일 주소 항목에 메일 주소가 등록되어 있지 않음

<figure><img src="../../.gitbook/assets/image (322).png" alt="" width="563"><figcaption></figcaption></figure>



❷ 보낸사람 항목에 표시된 사용자명을 탭합니다. 보낸사람 선택이 표시됩니다.<br>

<figure><img src="../../.gitbook/assets/image (316).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

3. '이메일 주소 추가'를 탭합니다.

<figure><img src="../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>



4. 메일 주소 항목에서 'Sign in with Gmail'을 탭합니다. Gmail 계정 선택 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (297).png" alt="" width="313"><figcaption></figcaption></figure>

&#x20;     &#x20;

5. 메일 전송에 사용할 계정을 탭합니다.

<div align="right"><figure><img src="../../.gitbook/assets/image (298).png" alt="" width="563"><figcaption></figcaption></figure></div>

인증이 완료되면 Gmail 인증 완료 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (299).png" alt="" width="319"><figcaption></figcaption></figure>



6. DirectCloud 애플리케이션으로 돌아가 필요에 따라 이름을 입력합니다.

{% hint style="info" %}
**NOTE**\
이름 항목에 입력한 문자는 링크, 업로드 요청, 첨부 파일 전송, Guest 초대, Connect User 초대의 알림 메일의 수신자, 제목, 본문에서 DirectCloud의 사용자명 대신 표시됩니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (300).png" alt="" width="334"><figcaption></figcaption></figure>



7. 필요에 따라 서명에서 추가를 선택하고, 메일 본문의 하단에 추가할 텍스트를 입력합니다.

<figure><img src="../../.gitbook/assets/image (319).png" alt="" width="375"><figcaption></figcaption></figure>



8. 설정한 메일 주소를 기본 메일 주소로 사용하려면 기본 메일 주소로 설정 토글 스위치를 켜고, 오른쪽 상단의 추가를 탭합니다.\
   다른 발신 메일 주소를 지정할 수 없는 경우에는 토글 스위치를 끌 수 없습니다.

<figure><img src="../../.gitbook/assets/image (301).png" alt="" width="404"><figcaption></figcaption></figure>



9. Gmail로 발송된 테스트 메일을 확인합니다.

<figure><img src="../../.gitbook/assets/image (302).png" alt="" width="455"><figcaption></figcaption></figure>



10. 이메일 주소가 발신자 선택 목록에 추가되었는지 확인합니다.
