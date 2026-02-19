---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/guest_bulk_edit
---

# Guest 정보를 일괄 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

템플릿에 맞춰 Guest 정보 변경용 CSV 파일을 작성한 후 업로드하면, 여러 Guest의 정보를 한 번에 변경할 수 있습니다.\
이 매뉴얼에서는 ‘Guest' 관리 메뉴의 ‘Guest 일괄 등록’에서 Guest 정보를 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
*   수정 대상 사용자 ID가 등록되어 있지 않은 경우에는 ‘등록되지 않은 사용자 ID입니다.’라는 오류가 표시됩니다.

    Guest 추가에 대해서는 [Guest를 일괄 등록하는 방법](https://help.directcloud.net/admin_manual/user/guest_bulk_register)을 참고해 주시기 바랍니다.
* CSV 업로드 처리 중에는 추가로 CSV 업로드를 다시 요청할 수 없습니다.
*   문자 코드가 ‘Shift\_JIS’인 CSV 파일 또는 텍스트 파일에\
    X 0213:2004(JIS2004) 규격으로 변경된 구자체 문자를 입력하면, 저장 시 글자가 깨질 수 있습니다.\
    이 상태 그대로 CSV 파일이나 텍스트 파일을 업로드하면, 깨진 글자 상태로 그대로 등록됩니다.

    이러한 문자 깨짐을 방지하기 위해 문자 코드는 UTF-8(BOM 포함)을 사용하는 것을 권장합니다.
*   ‘Guest 일괄 등록’ 화면에서 다운로드되는 CSV 파일의 문자 코드는 ‘환경 설정’ > ‘상세 설정’ 메뉴의 ‘문자 인코딩’설정에서 지정된 값이 적용됩니다.

    자세한 내용은 [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참고해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Guest 일괄 등록 화면 표시**
{% endhint %}

1. '계정 관리' > 'Guest' 메뉴를 선택하고 'Guest 관리' 탭을 선택한 다음 'Guest 일괄 등록' 버튼을 클릭합니다.\
   Guest 일괄 등록 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1776).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Guest 일괄 등록 템플릿 다운로드**
{% endhint %}

1. 'Guest 일괄 등록' 화면의 'CSV 업로드' 설정에서 샘플 양식 버튼을 클릭합니다.\
   CSV 파일 템플릿이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1777).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Guest 정보 변경을 위한 CSV 파일 만들기**
{% endhint %}

1. 다운로드한 템플릿을 편집하여 Guest 정보 변경을 위한 CSV 파일을 만듭니다.

<figure><img src="../../.gitbook/assets/image (1778).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="127">항목</th><th width="486">설명</th><th>필수여부</th></tr></thead><tbody><tr><td>사용자 ID</td><td>로그인할 때 Guest를 식별하는 데 사용되는 ID로 이메일 주소를 6~250자 이내로 설정합니다.<br>사용 가능한 문자: 영숫자, 기호(-_@.+#)</td><td>○</td></tr><tr><td>비밀번호</td><td>Guest 로그인 암호 문자열을 암호 정책에 따라 설정합니다.</td><td> </td></tr><tr><td>이름</td><td>Guest의 표시 이름을 250자 이내로 설정합니다.<br>사용 가능한 문자:<br>UTF-8의 한자, 한글, 영문대 문자, 숫자, 공백, 다국어 문자, 기호 및 이모티콘 등</td><td>○</td></tr><tr><td>전화번호</td><td>Guest 전화 번호를 50자 이내로 설정합니다.<br>사용 가능한 문자: 숫자, 기호(+-)</td><td> </td></tr><tr><td>회사명</td><td>Guest가 속한 회사명을 250자 이내로 설정합니다.<br>사용 가능한 문자:<br>UTF-8의 한자, 한글, 영문대 문자, 숫자, 공백, 다국어 문자, 기호 및 이모티콘 등</td><td>○</td></tr><tr><td>언어</td><td><p>다음 언어로 'jpn'(일본어), 'eng'(영어), 'kor'(한국어) 중 하나를 설정합니다.</p><ul><li>사용자 페이지 표시</li><li>Guest에게 보내는 알림 메일</li></ul></td><td> </td></tr><tr><td>상태</td><td>Guest의 상태를 설정합니다.<br>"Y" 또는 입력되지 않은 상태에서 활성화되고 "N"으로 비활성화됩니다.</td><td> </td></tr><tr><td>접속제어</td><td>Guest에게 '응용 프로그램', '장치 관리', '이중 인증', 'IP 주소'를 통한 액세스 제어를 적용합니다.<br>필요한 경우 '보안 정책' > '접속 제어 개별설정' 메뉴의 설정 이름을 지정합니다.<br>기본값은 "기본 설정"입니다.</td><td> </td></tr><tr><td>비밀번호 등록 이메일 보내기</td><td>비밀번호 등록 이메일을 보낼지 여부를 설정합니다.<br>「Y」를 입력하면 패스워드 등록용 메일을 송신합니다.<br>"N" 또는 입력하지 않은 경우 비밀번호 등록 이메일이 전송되지 않습니다.</td><td> </td></tr></tbody></table>



{% hint style="warning" %}
**Guest 정보 변경을 위한 CSV 파일 업로드**
{% endhint %}

1. ‘Guest 일괄 등록’ 화면의 ‘CSV 업로드’ 설정에서 ‘Guest 수정’을 선택한 후, ‘파일 선택’ 버튼을 클릭하여 작성한 Guest 정보 변경용 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2518).png" alt=""><figcaption></figcaption></figure>



2. '업로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2519).png" alt=""><figcaption></figcaption></figure>



3.  CSV 업로드 확인 화면에서 ‘파일명’, ‘등록 행 수’, ‘처리 유형’을 확인한 후 ‘바로 신청’ 버튼을 클릭합니다.

    ‘이메일로 접수 신청서 발행’ 버튼을 클릭한 경우에는 이 매뉴얼의 \<Guest 정보 변경 최종 신청 제출>의 절차에 따라 최종신청을 전송한 후 Guest를 업로드해 주시기 바랍니다.

<figure><img src="../../.gitbook/assets/image (1781).png" alt=""><figcaption></figcaption></figure>



4. CSV 파일에 기재된 Guest 정보가 변경됩니다. \
   Guest 정보 변경이 완료되면 "Guest 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1782).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Guest 정보 변경 최종 신청 제출**
{% endhint %}

Guest 수정용 CSV 파일 업로드에서 ‘이메일로 접수 신청서 발행’을 선택한 경우에는, 업로드 요청을 생성한 계약 담당 관리자 또는 일반 관리자의 이메일 주소로 최종 신청용 링크가 포함된 안내 메일이 발송됩니다.\
아래 절차에 따라 최종 신청을 전송하고 Guest정보를 변경해 주시기 바랍니다.

1. 안내 메일을 열고 ‘일괄등록 접수하기' URL을 클릭합니다.\
   '일괄등록 신청'화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1783).png" alt=""><figcaption></figcaption></figure>



2. '신청' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1784).png" alt=""><figcaption></figcaption></figure>



3. CSV 파일이 업로드되며, 파일에 기재된 Guest 정보가 변경됩니다. \
   Guest 정보 변경이 완료되면 "Guest 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1785).png" alt=""><figcaption></figcaption></figure>
