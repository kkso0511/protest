---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/custom_settings/change_email_address
---

# DirectCloud에서 발송하는 메일 주소를 자신의 메일 주소로 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

공유 링크나 첨부 파일을 전송할 때는 기본적으로 \<no-reply@directcloud.jp>라는 메일 주소로 DirectCloud의 메일 서버에서 발송됩니다.\
이 매뉴얼에서는 송신 메일 서버 설정에서 본인의 메일 주소를 사용해 DirectCloud에서 메일을 발송하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정' 메뉴를 사용할 수 있습니다.
* 아래 기능에서 메일을 보낼 때 발신 메일 주소를 변경할 수 있습니다.
  * 공유 링크
  * 파일첨부 메일 발송
  * Guest 초대
  * Connect User 초대
  * 업로드 요청
* 메일 서버에 따라 송신 서버(SMTP 서버)로 설정할 수 없거나, 보안 설정을 변경해야 하는 경우가 있을 수 있습니다. 자세한 내용은 메일 서버 관리자에게 문의하시기 바랍니다.
* 송신 메일 서버 설정이 표시되지 않는 경우, 관리 페이지의 표시 언어를 한국어 또는 영어로 설정한 상태에서 웹 브라우저의 자동 번역 기능이 작동하고 있을 가능성이 있습니다.\
  이 경우 브라우저의 자동 번역 기능을 비활성화하고 캐시를 모두 삭제한 뒤 다시 표시해주시기 바랍니다.
* 기본 발신 주소에서 자체 메일 주소로 변경하면 아래 기능을 사용할 수 있습니다.
  * 11명 이상의 수신자에게 전송
  * 반송 메일 수신
* 송신 메일 서버를 일괄 등록하는 것은 불가능합니다.
* 계정 설정 테스트를 수행하면 입력한 메일 주소와 사용자 ID가 화면에 남아 보일 수 있지만, 비밀번호를 포함한 해당 정보가 시스템에 저장되지는 않습니다.
* 송신 서버 항목에는 IP 주소를 등록할 수 없습니다.
* 기본 발신 메일 주소는 기본으로 사용함으로 설정되어 있습니다.
* 테스트 메일 전송에 실패하는 경우, 다음과 같은 원인을 고려할 수 있습니다.
  * 원인 1: 송신 서버 정보 입력 오류\
    올바른 송신 서버 정보를 입력해야 합니다.
  * 원인 2: 계정 설정 테스트 입력 오류\
    DirectCloud의 사용자 ID·비밀번호가 아니라, 본인이 사용하는 메일 서버의 사용자 ID·비밀번호가 입력되어 있는지 확인해야 합니다.
  *   원인 3: 메일 서버 측에서 외부 접근을 차단하고 있음\
      메일 서버의 보안 설정에 따라 접근이 차단될 수 있습니다.\
      메일 서버 설정에서 SMTP 접근을 허용한 뒤 다시 테스트해야 합니다.

      메일 서버에서 IP 주소 제한을 설정한 경우에는 54.64.42.47에서의 접근을 허용해야 합니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**메일 발신 서버 설정**
{% endhint %}

1. '공유 설정' > '맞춤형 설정' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 보내는 '이메일 발신서버' 설정에서 서버 정보의 방식을 수동설정으로 선택합니다.

<figure><img src="../../.gitbook/assets/image (447).png" alt=""><figcaption></figcaption></figure>



3. 메일을 보내는 데 사용할 서버의 정보를 입력합니다.

<figure><img src="../../.gitbook/assets/image (448).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="241">항목</th><th>설명</th></tr></thead><tbody><tr><td>보내는 메일 서버 (SMTP)</td><td>메일을 보내는 데 사용할 보내는 메일 서버(SMTP 서버)를 입력합니다.</td></tr><tr><td>포트</td><td><p>아웃바운드 메일 서버(SMTP 서버)의 포트 번호를 선택합니다.<br>각 포트 번호는 다음 용도로 사용됩니다.</p><ul><li>587:<br>TLS(Transport Layer Security)로 암호화하는 경우 일반적으로 포트 번호에 "587"을 지정합니다.</li><li>465:<br>SMTPS(SSL over SSL)를 제공하는 메일 서버에서 지정합니다.</li><li>25:<br>인증 기능이 없는 SMTP입니다. 대부분의 메일 서버에서 차단되므로 일반적으로 사용할 수 없습니다.</li></ul></td></tr><tr><td>보안연결</td><td>송신 서버에서 사용하는 암호화 통신으로 "SSL" "TLS" 중 하나를 선택합니다.</td></tr><tr><td>발신수 제한</td><td>대상에 한 번에 설정할 수 있는 최대 이메일 주소 수를 설정하려면 사용을 선택하고 하나 이상의 값을 입력합니다.</td></tr></tbody></table>



4. 디폴트 송신메일 이메일 주소인 no-reply@directcloud.net 를 사용할 수 있는지 여부를 선택하고 저장 버튼을 클릭합니다. '사용 안함'을 선택한 경우 사용자는 이메일 작성 화면에서 이 문서의 단계에서 수동으로 설정한 이메일 주소를 설정해야 합니다.

<figure><img src="../../.gitbook/assets/image (449).png" alt=""><figcaption></figcaption></figure>



5. 계정 설정 테스트에서 설정한 메일 서버에 연결할 수 있는 이메일 주소, 사용자 ID, 비밀번호를 입력한 다음 테스트 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (450).png" alt=""><figcaption></figcaption></figure>



6. 입력한 이메일 주소로 테스트 이메일이 전송되었는지 확인합니다.



7. 보내는 메일 서버 설정으로 돌아가서 보내는 메일 서버 설정의 사용을 선택합니다.\
   설정은 즉시 저장됩니다.

<figure><img src="../../.gitbook/assets/image (451).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Web 브라우저 또는 DirectCloud 드라이브에서 보낸사람 메일 주소를 등록하기**
{% endhint %}

1.  사용자 페이지에서 [\[Web, Drive\] 링크를 생성해 공유하는 방법](https://help.directcloud.net/user_manual/file_share/wd_link_share), [파일을 이메일에 첨부하여 전송하는 방법](https://help.directcloud.net/user_manual/file_share/attachment_mail)

    , [사용자 페이지에서 Guest를 초대하는 방법](https://help.directcloud.net/user_manual/file_share/invitaion_guest), [Connect User를 초대하는 방법](https://help.directcloud.net/user_manual/file_share/invitaion_connect_user), [업로드 요청 폴더에 파일을 업로드하는 방법](https://help.directcloud.net/user_manual/file_share/upload_to_file_request), 첨부 파일 전송, Guest 초대, 업로드 요청 화면 중 하나를 표시합니다.



2. 아래 방법 중 하나로 발신 메일 주소를 등록하는 화면을 표시합니다.

❶ '이메일 주소를 추가해 주세요.' 라고 표시되는 경우는 아래 두 조건을 모두 충족할 때입니다. \
&#x20;     이 경우 '발신 메일 주소를 등록해 주세요.' 를 클릭합니다.\
\
・관리 페이지의 송신 메일 서버 설정에서 기본 발신 메일 주소가 사용하지 않음으로 설정되어 있음\
・메일 작성 화면의 발신 메일 주소 항목에 메일 주소가 등록되어 있지 않음

<figure><img src="../../.gitbook/assets/image (2321).png" alt="" width="421"><figcaption></figcaption></figure>



❷ 보낸사람 항목의 톱니바퀴 버튼을 클릭합니다. '보낸사람 이메일 주소'가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2322).png" alt=""><figcaption></figcaption></figure>

&#x20;   &#x20;

3. '이메일 주소 추가'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2324).png" alt=""><figcaption></figcaption></figure>



4. 이 매뉴얼의 발신 메일 서버를 설정하는 방법에서 설정한 메일 송신 서버의 메일 주소, 사용자 ID, 비밀번호를 입력합니다.

<figure><img src="../../.gitbook/assets/image (310).png" alt="" width="418"><figcaption></figcaption></figure>

{% hint style="info" %}
**NOTE**\
이름 항목에 입력한 문자는 링크, 업로드 요청, 첨부 파일 전송, Guest 초대, Connect User 초대의 알림 메일의 수신자, 제목, 본문에서 DirectCloud의 사용자명 대신 표시됩니다.
{% endhint %}



5. 필요에 따라 서명에서 추가를 선택하고, 메일 본문의 하단에 추가할 텍스트를 입력합니다.

<figure><img src="../../.gitbook/assets/image (311).png" alt=""><figcaption></figcaption></figure>



6. 설정한 메일 주소를 기본 메일 주소로 사용하려면 기본 메일 주소로 설정에 체크한 뒤 확인 버튼을 클릭합니다.\
   테스트 메일이 전송됩니다.\
   다른 발신 메일 주소를 지정할 수 없는 경우에는 이 체크를 해제할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

7. 다시 한 번 테스트 메일이 정상적으로 전송되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (313).png" alt=""><figcaption></figcaption></figure>



8. 보낸사람 이메일 주소가 추가된 것을 확인합니다.

<figure><img src="../../.gitbook/assets/image (314).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**모바일에서 보낸사람 메일 주소를 등록하기**
{% endhint %}

1. 사용자 페이지에서 [\[Mobile\] 링크를 생성해 공유하는 방법](https://help.directcloud.net/user_manual/file_share/m_link_share), [\[Mobile\] 계정이 없는 상대로부터 파일을 받는 방법(업로드 요청 기능)](https://help.directcloud.net/user_manual/file_share/m_file_request)에 따라 공유 링크 또는 업로드 요청 화면 중 하나를 표시합니다.<br>
2. 아래 방법 중 하나로 보낸사람 메일 주소를 등록하는 화면을 표시합니다.

❶ '이메일 주소가 필요합니다.' 라고 표시되는 경우는 아래 두 조건을 모두 충족할 때입니다. \
이 경우 '메일 주소를 등록해 주세요.' 를 탭합니다.

・관리 페이지의 송신 메일 서버 설정에서 기본 발신 메일 주소가 사용하지 않음으로 설정되어 있음\
・메일 작성 화면의 발신 메일 주소 항목에 메일 주소가 등록되어 있지 않음

<figure><img src="../../.gitbook/assets/image (322).png" alt="" width="563"><figcaption></figcaption></figure>



❷ 보낸사람 항목에 표시된 사용자명을 탭합니다. 보낸사람 선택이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (316).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

3. '이메일 주소 추가'를 탭합니다.

<figure><img src="../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>



4. 이 매뉴얼의 발신 메일 서버를 설정하는 방법에서 설정한 메일 송신 서버의 메일 주소, 사용자 ID, 비밀번호를 입력합니다.

<figure><img src="../../.gitbook/assets/image (318).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**NOTE**\
이름 항목에 입력한 문자는 링크, 업로드 요청, 첨부 파일 전송, Guest 초대, Connect User 초대의 알림 메일의 수신자, 제목, 본문에서 DirectCloud의 사용자명 대신 표시됩니다.
{% endhint %}



5. 필요에 따라 서명에서 추가를 선택하고, 메일 본문의 하단에 추가할 텍스트를 입력합니다.

<figure><img src="../../.gitbook/assets/image (319).png" alt="" width="375"><figcaption></figcaption></figure>



6. 설정한 메일 주소를 기본 메일 주소로 사용하려면 기본 메일 주소로 설정 토글 스위치를 켜고, 오른쪽 상단의 추가를 탭합니다.\
   테스트 메일이 전송됩니다.\
   다른 발신 메일 주소를 지정할 수 없는 경우에는 토글 스위치를 끌 수 없습니다.

<figure><img src="../../.gitbook/assets/image (320).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

7. 테스트 메일이 정상적으로 전송되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (321).png" alt=""><figcaption></figcaption></figure>



8. 보낸사람 이메일 주소가 추가된 것을 확인합니다.
