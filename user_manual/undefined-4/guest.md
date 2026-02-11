---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-4/guest
---

# 사용자 페이지에서 Guest를 초대하는 방법

### 개요 <a href="#a03" id="a03"></a>

Guest 추가 방법에는, 관리자가 Guest를 추가하는 방법 외에도, 사용자가 Guest를 초대하는 방법이 있습니다. 이 매뉴얼 에서는 사용자 페이지에서 Guest를 초대하는 방법에 대해 설명합니다.

***

### 동작조건

* 이 매뉴얼 에서는 Shared Box에서의 작업 절차를 설명하고 있지만, DLP 폴더에서도 동일한 방법으로 작업할 수 있습니다.  Connect 폴더, Warm Storage에서는 Guest를 초대할 수 없습니다.
* Guest를 초대하려면, 사용자에게 <마스터>, <전체권한> 접근 권한이 부여되어 있어야 합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Guest를 초대할 수 있는 사용자 수에는 제한이 없습니다.
* 사용자 ID와 Guest ID에 동일한 문자열을 설정할 수는 없습니다.
* Guest 등록용 URL의 유효 기간은, 이메일 초대든 링크 초대든 관계없이 관리자 페이지에서 설정한 기간으로 고정됩니다.
* 'Guest 초대' 화면의 '링크로 초대' 탭에 있는 '이메일 주소' 항목에 이미 등록된 Guest를 입력하면,\
  해당 Guest에 설정된 '회사명', '이름', '유효 기간' 값이 자동으로 입력되며, 이 항목들은 수정할 수 없도록 비활성화(회색 표시)됩니다.\
  Guest 초대용 링크를 통해 등록할 경우, 기존 Guest 정보는 새 정보로 덮어쓰기 됩니다.
* '받는 사람', '제목', '내용'을 입력한 뒤 'Guest 초대' 화면의 오른쪽 상단에 있는 '✕' 버튼 또는 '취소' 버튼을 클릭하면 입력한 설정 내용이 임시로 저장됩니다. 이후 동일한 폴더에서 “Guest 초대”를 클릭하고, 표시된 확인 화면에서 ‘확인’ 버튼을 클릭하면 이전에 저장된 설정 내용을 불러와 표시할 수 있습니다.
* 'Guest 초대' 화면의 '보내는 사람'에 표시되는 이름은\
  no-reply 메일에 회신할 수 있도록 설정되어 있는지 여부에 따라 다르게 표시됩니다.\
  · no-reply 메일에 회신할 수 있는 경우: 사용자 이름 no-reply@directcloud.jp\
  · no-reply 메일에 회신할 수 없는 경우: DirectCloud no-reply@directcloud.co.jp
* 비밀번호 끝에 반각 공백(스페이스)이 포함된 상태로 복사해 비밀번호 입력 화면에 붙여넣더라도, 공백은 자동으로 제거됩니다.
* Guest에게 설정할 수 있는 접근 권한은 일반 사용자 및 그룹과 동일합니다.\
  단, Guest는 다음 기능을 사용할 수 없습니다.\
  · 첨부파일 전송\
  · 업로드 요청\
  · Guest 초대\
  · Guest 초대 승인\
  · 접근 권한 설정\
  · 폴더 속성 설정
* 또한 Guest는 1단계(최상위) 폴더를 조작할 수 없기 때문에 Guest에게 <마스터> 권한을 부여할 수 없습니다.
* 사용자 페이지에서는 초대한 Guest 정보를 확인할 수 없습니다. \
  Guest의 정보는 관리자 페이지에서 확인할 수 있습니다.
* Guest가 설정할 수 있는 비밀번호 규칙, 비밀번호 유효 기간, 비밀번호 변경 정책 등은 관리자에 의해 정의됩니다.
* Guest가 비밀번호를 잊은 경우, 로그인 화면의 “비밀번호를 분실한 경우” 버튼을 클릭한 뒤\
  '비밀번호 재설정' 화면에서 'Guest 이신가요?'를 선택하여 비밀번호를 다시 설정하세요.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Guest 초대 화면 표시**
{% endhint %}

1. Shared Box 메뉴를 클릭하고 Guest를 초대할 첫 번째 계층 구조 이후의 폴더를 클릭한 다음 화면 오른쪽에 표시되는 슬라이드 메뉴에서 Guest 초대 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1066).png" alt=""><figcaption></figcaption></figure>

&#x20;      Guest 초대 화면이 표시됩니다.



{% hint style="warning" %}
**Guest 초대 화면 구성**
{% endhint %}

**\[메일로 초대]**

<figure><img src="../../.gitbook/assets/image (1067).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="109">No.</th><th width="242">항목</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>"메일로 초대"/ "링크로 초대"</td><td>이메일로 초대 탭과 링크로 초대 탭 사이를 전환합니다.</td></tr><tr><td>❷</td><td>보낸 사람</td><td>Guest 초대 화면에서 메일을 보낼 때 발신자를 설정합니다.</td></tr><tr><td>❸</td><td>받는 사람</td><td><p>Guest 초대 화면에서 Guest 초대를 위한 URL을 보낼 대상을 250자 이내로 설정합니다.<br>사용 가능한 문자: 반각 영숫자, 기호(-_@.+#)<br>대상은 최대 10개까지 설정할 수 있습니다.<br><br><strong>NOTE:</strong><br>여러 개의 이메일 주소를 구분 문자로 나열한 뒤, 텍스트 편집기 등에서 복사해 붙여 넣으면 한 번에 설정할 수 있습니다.<br>구분 문자로는 세미콜론(;), 콤마(,), 공백, 탭, 줄바꿈을 사용할 수 있으며, 혼합해서 사용해도 문제 없습니다.</p><p>이메일 주소는 “사용자명 &#x3C;이메일 주소>” 형식으로 지정할 수도 있습니다.<br><br>입력 예시 1:<br>user1 &#x3C;<a href="mailto:user1@example.com">user1@example.com</a>>, user2 &#x3C;<a href="mailto:user2@example.com">user2@example.com</a>>, user3 &#x3C;<a href="mailto:user3@example.com">user3@example.com</a>><br><br>입력 예시 2:<br><a href="mailto:user1@example.com">user1@example.com</a>; user2 &#x3C;<a href="mailto:user2@example.com">user2@example.com</a>>, &#x3C;<a href="mailto:user3@example.com">user3@example.com</a>></p></td></tr><tr><td>❹</td><td>제목</td><td>Guest 초대 화면에서 이메일을 보낼 때 이메일 제목을 입력합니다.<br>변경하지 않으면 "[DirectCloud] 000님이 귀하를 초대하였습니다."라는 제목으로 이메일이 전송됩니다.</td></tr><tr><td>❺</td><td>내용</td><td>“Guest 초대” 화면에서 링크 URL을 전송할 때, 이메일 본문에 추가할 문장을 입력할 수 있습니다.<br>내용을 변경하지 않으면, 기본적으로 다음 문구가 포함된 이메일이 전송됩니다.<br><br>"안녕하세요.<br>귀하를 DirectCloud의 Guest로 초대하고자 합니다. 아래 초대정보를 확인해보세요."</td></tr><tr><td>❻</td><td>언어 전환 버튼</td><td>받는 사람에 설정한 이메일 주소로 전송되는 이메일의 언어를 '일본어', '영어', '한국어' 중 하나로 전환합니다.<br>그러나 회사 이름, 보낸 사람 이름 및 폴더 경로는 선택한 언어로 변경되지 않습니다.<br>표시는 웹 브라우저의 언어 설정에 따라 다릅니다.</td></tr><tr><td>❼</td><td>관리자의 승인 정보</td><td>Guest 초대에 관리자가 승인해야 하는 경우 여기에 "초대장은 관리자(또는 마스터)가 승인해야 발송됩니다."라고 표시됩니다.</td></tr><tr><td>❽</td><td>위치</td><td>Guest를 초대한 폴더의 경로가 표시됩니다.</td></tr><tr><td>❾</td><td>권한</td><td>드롭다운 목록에서 Guest에게 부여할 권한을 선택합니다.</td></tr><tr><td>❿</td><td>유효기간</td><td>체크를 선택하면 Guest의 유효 기간을 설정할 수 있습니다.<br>날짜 입력란을 클릭한 후 표시된 달력에서 날짜를 선택하면 유효 기간을 지정할 수 있습니다.<br>여기서 설정한 유효 기간이 지나면, Guest는 해당 폴더에 접근할 수 없게 됩니다.</td></tr><tr><td>⓫</td><td>메모</td><td>메모를 입력하기 위한 텍스트 상자가 표시됩니다.<br>Guest에 대한 정보 등을 기록하는 데 사용할 수 있습니다.</td></tr><tr><td>⓬</td><td>미리보기 버튼</td><td>클릭하면 미리보기 화면에서 'Guest 초대' 화면에서 보낸 메일의 내용을 확인할 수 있습니다.</td></tr><tr><td>⓭</td><td>제출 버튼</td><td>설정한 Guest 초대를 위한 URL을 이메일로 보냅니다.</td></tr><tr><td>⓮</td><td>취소 버튼</td><td>설정을 취소하고 Guest 초대 화면을 닫습니다.</td></tr></tbody></table>



**\[링크로 초대 탭]**

<figure><img src="../../.gitbook/assets/image (1068).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="114">No.</th><th width="243">항목</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>"메일로 초대"/ "링크로 초대"</td><td>이메일로 초대 탭과 링크로 초대 탭 사이를 전환합니다.</td></tr><tr><td>❷</td><td>위치</td><td>Guest를 초대한 폴더의 경로가 표시됩니다.</td></tr><tr><td>❸</td><td>이메일 주소</td><td>Guest 초대 화면에서 Guest 초대를 위한 URL을 보낼 대상을 설정합니다.<br>조회 버튼을 클릭하면 회사 이름 이후의 텍스트 상자에 문자를 입력할 수 있습니다.</td></tr><tr><td>❹</td><td>회사명</td><td>Guest  속한 회사명을 설정할 수 있습니다.<br>Guest  등록 화면에서 Guest  정보를 등록하는 단계에서 Guest 가 변경할 수도 있습니다.</td></tr><tr><td>❺</td><td>이름</td><td>게스트의 이름을 설정할 수 있습니다.<br>게스트 등록 화면에서 게스트 정보를 등록하는 단계에서 게스트가 변경할 수도 있습니다.</td></tr><tr><td>❻</td><td>권한</td><td>드롭다운 목록에서 Guest에게 부여할 접근 권한을 선택합니다.</td></tr><tr><td>❼</td><td>유효기간</td><td>체크를 선택하면 Guest의 유효 기간을 설정할 수 있습니다.<br>날짜 입력란을 클릭해 표시된 달력에서 날짜를 선택하면 유효 기간을 지정할 수 있습니다.<br>여기서 설정한 유효 기간이 지나면, Guest는 해당 폴더에 접근할 수 없습니다.</td></tr><tr><td>❽</td><td>메모</td><td>Guest 관련 정보를 기록할 수 있는 메모 입력란이 표시됩니다.</td></tr><tr><td>❾</td><td>관리자의 승인 정보</td><td>Guest 초대에 관리자가 승인해야 하는 경우 여기에 "초대장은 관리자(또는 마스터)가 승인해야 발송됩니다."라고 표시됩니다.</td></tr><tr><td>❿</td><td>링크생성 버튼</td><td>설정한 내용으로 Guest 초대를 위한 URL을 만듭니다.</td></tr><tr><td>⓫</td><td>취소 버튼</td><td>설정을 취소하고 Guest 초대 화면을 닫습니다.</td></tr></tbody></table>



{% hint style="warning" %}
**이메일로 Guest 초대**
{% endhint %}

이 매뉴얼에서는 이메일로  Guest 초대를 하는 기본 단계에 대해 설명합니다.

1. Guest 초대 화면에서 이메일로 초대 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1069).png" alt=""><figcaption></figcaption></figure>



2. '받는 사람'에 링크를 보낼 이메일 주소를 입력합니다.\
   입력란 이외의 장소를 클릭하면 입력한 이메일 주소가 반영됩니다.\
   개인/회사 주소록을 사용하도록 설정하는 방법 에 따라 주소록이 활성화된 경우 오른쪽에 표시된 아이콘을 클릭하여 주소록에서 대상 이메일 주소를 선택할 수도 있습니다.&#x20;

<figure><img src="../../.gitbook/assets/image (1070).png" alt=""><figcaption></figcaption></figure>



3. 필요한 경우 제목과 내용을 입력합니다.

<figure><img src="../../.gitbook/assets/image (1071).png" alt=""><figcaption></figcaption></figure>



4. 권한 드롭다운 목록에서 Guest에 할당할 접근 권한을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1072).png" alt=""><figcaption></figcaption></figure>



5. 필요한 경우 Guest의 만료 날짜를 설정합니다.

<figure><img src="../../.gitbook/assets/image (1073).png" alt=""><figcaption></figcaption></figure>



6. 전송되는 이메일의 내용을 확인하려면 미리보기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1074).png" alt=""><figcaption></figcaption></figure>

메일 내용이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1075).png" alt=""><figcaption></figcaption></figure>



7. 설정한 내용으로 링크를 보낼 수 있는 경우에는 '보내기' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1076).png" alt=""><figcaption></figcaption></figure>

Guest 초대 이메일이 전송됩니다.



**\[관리자의 승인이 필요한 경우]**

관리자 설정에서 관리자 또는 보조 관리자가 승인한 후 Guest에게 초대 이메일을 보내도록 설정된 경우 계약 담당 관리자, 일반 관리자가 Guest 초대를 승인하면 다음과 같은 "Guest 초대 승인 요청이  있습니다."라는 제목의 알림 이메일이 전송됩니다. 또한 초대된 사용자에게 Guest 초대 이메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (1083).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**링크로 Guest 초대**
{% endhint %}

이 매뉴얼에서는 Guest  초대 URL을 생성하는 기본 단계에 대해 설명합니다.

1. Guest 초대 화면에서 링크로 초대 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1077).png" alt=""><figcaption></figcaption></figure>



2. 이메일 주소에 Guest로 초대할 사용자의 이메일 주소를 입력하고 조회 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1078).png" alt=""><figcaption></figcaption></figure>

회사명 이후의 항목을 설정할 수 있습니다.



3. 권한 드롭다운 목록에서 Guest에 할당할 접근 권한을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1079).png" alt=""><figcaption></figcaption></figure>



4. 필요한 경우 Guest의 만료 날짜를 설정합니다.

<figure><img src="../../.gitbook/assets/image (1080).png" alt=""><figcaption></figcaption></figure>



5. 링크생성 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1082).png" alt=""><figcaption></figcaption></figure>

화면 오른쪽 영역에 게시된 Guest 초대를 위한 URL이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1085).png" alt=""><figcaption></figcaption></figure>



6. Guest 초대 URL의 '복사' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1086).png" alt=""><figcaption></figcaption></figure>

클립보드에 Guest 등록 화면에 대한 링크 정보가 복사됩니다.



7. 복사한 정보를 메시징 응용 프로그램 작성 화면 등에 붙여넣고 초대 대상으로 보냅니다.



**\[관리자의 승인이 필요한 경우]**

'복사' 버튼의 왼쪽에 '대기 중'이 표시되면 계약 담당 관리자, 일반 관리자의 승인을 기다려야 합니다.

<figure><img src="../../.gitbook/assets/image (1084).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Guest 등록 화면에서 Guest 정보 등록**
{% endhint %}

'메일로 Guest 초대' 절차에 따라 Guest를 초대하면 대상에 설정한 사용자에게 "\[DirectCloud] 000님이 귀하를 초대하였습니다."라는 제목의 Guest 초대 이메일이 전송됩니다. 이메일을 받은 사용자는 다음 절차에 따라 Guest 등록을 할 수 있습니다.

1. 다음 방법 중 하나로 미리보기 화면을 표시합니다.

❶ Guest 초대 이메일을 보고 Guest 초대 URL 링크를 클릭

<figure><img src="../../.gitbook/assets/image (1087).png" alt=""><figcaption></figcaption></figure>

❷ '링크로 Guest 초대' 절차에 따라 Guest를 초대한 경우 'Guest 로그인'에서 링크를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1090).png" alt=""><figcaption></figcaption></figure>

Guest 등록 화면이 표시됩니다.



2. 설정하려는 회사명, 이름, 비밀번호를 입력하고 등록 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1088).png" alt=""><figcaption></figcaption></figure>



3. 'Guest 회원으로 가입이 완료되었습니다.'라는 메시지가 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1092).png" alt=""><figcaption></figcaption></figure>



4. '로그인 페이지로 이동' 버튼을 클릭하면 로그인 화면에 액세스할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1093).png" alt=""><figcaption></figcaption></figure>
