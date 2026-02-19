---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_share/attachment_mail
---

# 파일을 이메일에 첨부하여 전송하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 파일을 이메일에 첨부하여 전송하는 방법을 설명합니다.\
이메일에 첨부된 파일은 ZIP 형식으로 압축되어 전송됩니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 공유 폴더에서의 작업 방법을 기준으로 설명하고 있지만, My Box, DLP 폴더에서도 동일한 절차로 사용할 수 있습니다.
* 관리자가 사용 권한 설정에서 ‘Email’ 항목에 체크된 권한 세트를 그룹과 사용자에게 부여해야 합니다.
* 첨부파일 전송 기능을 사용하려면 <마스터>, <전체권한>, <편집자> 접근 권한이 필요합니다.
* 첨부파일 전송으로 송부할 수 있는 파일의 용량 상한은 합계로 7MB입니다.
* 첨부파일 전송으로 보낼 수 있는 파일의 최대 용량은 총 7MB입니다.
* 생성된 ZIP 형식 파일은 다른 메일 프로그램에 첨부하여 전송할 수 없습니다.
* 폴더 자체를 첨부하여 전송하는 것도 불가능합니다.
* Guest는 첨부파일 전송을 이용할 수 없습니다.
* 다음 폴더에서는 첨부파일 전송 기능을 이용할 수 없습니다.
  * Connect 폴더
  * Warm Storage 폴더
  * Cold Storage 폴더
* "받는 사람", "참조 / 숨은참조" "제목", "내용"을 입력한 후 첨부파일 전송 화면의 오른쪽 상단에 있는 X 버튼 또는 취소 버튼을 클릭하면, 설정 내용이 임시로 저장됩니다.\
  이후 동일한 폴더에서 첨부파일 생성을 다시 시작하고 표시된 화면에서 확인 버튼을 클릭하면, 이전에 저장된 설정 내용을 불러올 수 있습니다.
* 첨부파일 전송 화면의 발신자 이름은 no-reply 메일에 회신할 수 있는지 여부에 따라 다르게 표시됩니다.
  * no-reply 메일에 회신할 수 있는 경우: 사용자 이름 no-reply@directcloud.jp
  * no-reply 메일에 회신할 수 없는 경우: DirectCloud no-reply@directcloud.co.jp
* 옵션 ‘DirectCloud-CONNECT’를 사용할 수 있는 경우, 사용자 페이지에 Connect 메뉴가 표시됩니다.
* 옵션 ‘DirectCloud-SHIELD DLP’를 계약한 경우, 사용자 페이지에 DLP 메뉴가 표시됩니다.
* DLP 폴더의 파일을 ZIP 형식으로 압축해 전송하려면, DLP 설정에서 ‘첨부파일 전송 설정’의 ‘사용함’ 항목에 체크가 되어 있어야 합니다.
* Warm Storage를 이용할 수 있는 경우, 사용자 페이지에 Warm Storage 메뉴가 표시됩니다.
* 옵션인 Cold Storage를 계약한 경우, 사용자 페이지에 Cold Storage 메뉴가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**첨부파일 전송 기능으로 파일을 압축하여 전송**
{% endhint %}

**\[첨부파일 전송 화면 표시]**

1. 압축하고 전송할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1123).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나를 사용하여 '파일첨부 메일발송' 화면을 표시합니다.

❶  압축하여 보내고 싶은 파일을 체크하고 왼쪽 상단의 '파일첨부 메일발송' 버튼을 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1124).png" alt=""><figcaption></figcaption></figure>

❷  압축하여 보내고 싶은 파일을 체크하고 오른쪽 클릭하여 표시된 메뉴에서 '파일첨부 메일발송'를 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1125).png" alt=""><figcaption></figcaption></figure>

❸  압축하여 보내려는 파일의 오른쪽에 있는 ▼ 버튼을 클릭하고 표시된 메뉴에서 '파일첨부 메일발송'을 클릭합니다. 여러 파일을 선택할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (1126).png" alt=""><figcaption></figcaption></figure>

파일첨부 메일발송 화면이 나타납니다.



**\[파일첨부 메일발송 화면의 기본 구성]**

<figure><img src="../../.gitbook/assets/image (1127).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="123">No.</th><th width="143">항목</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>보낸 사람</td><td>첨부파일 보내기 화면에서 첨부파일이 있는 메일을 보낼 때 발신자를 설정합니다.</td></tr><tr><td>❷</td><td>받는 사람</td><td>첨부파일 보내기 화면에서 첨부파일이 있는 메일을 보낼 때의 수신처를 250자 이내로 설정합니다.<br>사용 가능한 문자: 영숫자, 기호(-_@.+#)<br>대상은 최대 10개까지 설정할 수 있습니다.</td></tr><tr><td>❸</td><td>참조/숨은참조</td><td>클릭하면 Cc 및 Bcc 대상 이메일 주소를 입력하는 양식이 표시됩니다.</td></tr><tr><td>❹</td><td>제목</td><td>첨부파일 보내기 화면에서 첨부파일이 있는 메일을 보낼 때 메일의 제목을 입력합니다.<br>변경하지 않는 경우는, 「[DirectCloud] 00님이 첨부파일을 전송했습니다.」라고 하는 제목으로 메일이 송신됩니다. </td></tr><tr><td>❺</td><td>내용</td><td>첨부파일 보내기 화면에서 첨부파일이 있는 메일을 보낼 때 메일 본문에 추가할 문장을 입력합니다.</td></tr><tr><td>❻</td><td>언어 전환 버튼</td><td>받는 사람에 설정한 이메일 주소로 전송되는 이메일의 언어를 '일본어', '영어', '한국어' 중 하나로 전환합니다.<br>그러나 회사 이름, 보낸 사람 이름, 본문은 선택한 언어로 변경되지 않습니다. 표시는 웹 브라우저의 언어 설정에 따라 다릅니다.</td></tr><tr><td>❼</td><td>첨부파일</td><td>선택한 첨부 파일의 정보가 표시됩니다.<br>여러 파일을 선택한 경우에만 파일 오른쪽에 표시된 ✕ 버튼을 클릭하면 첨부 파일에서 제거할 수 있습니다.</td></tr><tr><td>❽</td><td>비밀번호</td><td>첨부 파일을 압축 해제할 때 암호를 설정합니다.<br>표준에서는 8자 암호가 자동으로 생성되도록 설정됩니다.<br>문자 유형, 문자 수 및 사용 가능한 기호에는 제한이 없지만 반각으로 입력해야 합니다.<br>비밀번호를 선택 해제할 수 없습니다.</td></tr><tr><td>❾</td><td>옵션</td><td><p>드롭다운 목록에서 업로드 요청의 링크 URL에 액세스할 수 있는 비밀번호를 보내는 방법을 선택합니다. 비밀번호를 보내는 방법은 다음과 같습니다.<br></p><ul><li>비밀번호 별도 이메일 발송: 비밀번호가 포함된 이메일을 대상에 다른 이메일로 보냅니다.</li><li>비밀번호 동봉 발송: 비밀번호를 링크 메일에 기재하여 보냅니다.</li><li>비밀번호를 보낸 사람에게만 발송: 비밀번호가 포함된 이메일을 보낸 사람(발신자)에게 보냅니다.</li><li>비밀번호 미발송: 비밀번호를 보내지 않고 링크만 포함된 이메일을 보냅니다.</li></ul></td></tr><tr><td>❿</td><td>미리보기 버튼</td><td>클릭하면 미리보기 화면에서 "첨부 파일 보내기" 화면에서 보낸 메일의 내용을 확인할 수 있습니다.</td></tr><tr><td>⓫</td><td>보내기 버튼</td><td>설정한 내용으로 첨부파일이 있는 메일을 보냅니다.</td></tr><tr><td>⓬</td><td>취소 버튼</td><td>설정을 취소하고 "첨부 파일 보내기" 화면을 닫습니다.</td></tr></tbody></table>



**\[첨부파일 보내기]**

1. '파일첨부 메일발송' 화면에서 받는 사람에 첨부파일을 보낼 이메일 주소를 입력합니다. 입력란 이외의 장소를 클릭하면 입력한 이메일 주소가 반영됩니다. \
   [회사·개인 주소록을 활성화하는 방법](https://help.directcloud.net/admin_manual/detail_settings/enable_addressbook)에 따라 주소록이 활성화된 경우 오른쪽에 표시된 아이콘을 클릭하여 주소록에서 대상 이메일 주소를 선택할 수도 있습니다.&#x20;

<figure><img src="../../.gitbook/assets/image (1128).png" alt=""><figcaption></figcaption></figure>



2. 필요한 경우 제목과 내용을 입력합니다.

<figure><img src="../../.gitbook/assets/image (1129).png" alt=""><figcaption></figcaption></figure>



3. 전송되는 이메일의 내용을 확인하려면 미리보기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1130).png" alt=""><figcaption></figcaption></figure>



4. 이메일 내용을 확인하고 ✕ 버튼을 클릭하여 미리보기를 닫습니다.

<figure><img src="../../.gitbook/assets/image (1131).png" alt=""><figcaption></figcaption></figure>



5. 설정한 내용으로 첨부파일이 있는 메일을 보낼 수 있다면 '보내기' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1132).png" alt=""><figcaption></figcaption></figure>

&#x20;      이메일이 전송됩니다.



{% hint style="warning" %}
**파일첨부 메일발송으로 발송된 압축 파일을 해제하기**
{% endhint %}

1. "\[DirectCloud] 00님이 첨부파일을 전송했습니다." 라고 하는 제목 메일을 클릭 후, 첨부된 ZIP 형식의 파일을 다운로드합니다.

<figure><img src="../../.gitbook/assets/image (1133).png" alt=""><figcaption></figcaption></figure>



2. 축 해제 소프트웨어를 사용하여 다운로드한 파일의 압축을 풉니다.\
   비밀번호가 설정된 링크 메일의 경우, 압축 해제 도중에 비밀번호 입력 화면이 표시됩니다.\
   비밀번호 입력 화면이 표시되지 않으면 4단계로 진행합니다.



3. 비밀번호를 보내는 방법에 따라 비밀번호를 입력합니다.

❶  첨부 파일 첨부 메일의 패스워드의 송신 방법으로서 '비밀번호 별도 이메일 발송'을 선택한 경우 첨부 파일 첨부의 메일과는 별도로 "00님이 발송한 첨부파일의 비밀번호입니다." 라는 건명 메일이 도착합니다.\
해당 이메일에 나열된 '비밀번호'를 입력하고 '확인' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1134).png" alt=""><figcaption></figcaption></figure>

❷  첨부파일이 있는 메일의 비밀번호를 보내는 방법으로 '비밀번호 동봉 발송'을 선택한 경우\
첨부파일이 있는 메일에 기재된 비밀번호를 입력하고 '확인' 버튼을 클릭합니다.\
첨부 파일이 추출되고 폴더가 검색됩니다.



4. 압축이 해제된 폴더를 두 번 클릭합니다.\
   압축을 푼 파일이 표시됩니다.
