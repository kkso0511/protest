---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/bulk_register
---

# 다수의 사용자를 일괄 등록하는 방법

### 개요 <a href="#a03" id="a03"></a>

템플릿에 맞춰 사용자 정보 변경용 CSV 파일을 작성한 후 업로드하면, 여러 사용자의 정보를 한 번에 변경할 수 있습니다.\
이 매뉴얼에서는 ‘계정 관리’ 메뉴의 ‘사용자 일괄 처리’에서 사용자 정보를 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항  <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* 사용자 추가용 CSV 파일에서 비밀번호 등록용 메일 보내기를 비활성화(N 입력)로 설정하고, 비밀번호 항목에 비밀번호 문자열을 입력한 상태로 파일을 등록하면, 추가된 사용자 ID로 사용자 페이지에 로그인할 때 비밀번호 변경 화면이 표시됩니다.
* 사용자에게 발송된 알림 메일을 통해 비밀번호를 등록했거나, 관리 페이지의 URL 복사 기능을 통해 비밀번호가 등록된 경우에는 비밀번호 변경 화면이 표시되지 않습니다.
*   각 그룹은 두 자리 그룹 코드로 관리되며, 그룹을 생성할 때는 부모 그룹 코드 두 자리와 새로 부여되는 그룹 코드 두 자리가 합쳐져 등록됩니다.\
    예를 들어 회사명 폴더의 그룹 코드가 AA인 경우, 해당 폴더 바로 아래에 첫 번째 그룹을 만들면 AAAA가, 두 번째 그룹을 만들면 AAAB가 그룹 코드로 등록됩니다.

    두 자리 그룹 코드는 아래와 같은 조합으로 구성되며, 이를 모두 합치면 최대 3,844개의 그룹을 생성할 수 있습니다.

    <table><thead><tr><th width="126.20001220703125" align="center">No.</th><th align="center">코드 구분</th><th align="center">범위</th><th align="center">그룹 수</th></tr></thead><tbody><tr><td align="center">1</td><td align="center">영문 대문자만</td><td align="center">AA～ZZ </td><td align="center">676</td></tr><tr><td align="center">2</td><td align="center">영문 대문자＋소문자</td><td align="center">Aa～Zz</td><td align="center">676</td></tr><tr><td align="center">3</td><td align="center">영문 대문자＋숫자</td><td align="center">A0～A9</td><td align="center">260</td></tr><tr><td align="center">4</td><td align="center">영문 소문자＋대문자</td><td align="center">aA～zZ</td><td align="center">676</td></tr><tr><td align="center">5</td><td align="center">영문 소문자만</td><td align="center">aa～zz</td><td align="center">676</td></tr><tr><td align="center">6</td><td align="center">영문 소문자＋숫자</td><td align="center">a0～a9</td><td align="center">260</td></tr><tr><td align="center">7</td><td align="center">숫자＋영문 대문자</td><td align="center">0A～9A</td><td align="center">260</td></tr><tr><td align="center">8</td><td align="center">숫자＋영문 소문자</td><td align="center">0a～9a</td><td align="center">260</td></tr><tr><td align="center">9</td><td align="center">숫자만</td><td align="center">00～99</td><td align="center">100</td></tr></tbody></table>
* 이미 동일한 사용자 ID가 등록되어 있는 경우 등록된 사용자 ID입니다라는 오류가 표시됩니다.
* 가져오기 작업이 진행되는 동안에는 추가로 CSV 가져오기를 요청할 수 없습니다.
* 또한 문자 인코딩이 Shift\_JIS인 CSV 파일이나 텍스트 파일에 X 0213:2004(JIS2004) 규격으로 변경된 옛 한자를 입력하면 저장 시 문자가 깨집니다. 이러한 상태로 CSV 파일이나 텍스트 파일을 가져오면 깨진 문자 그대로 가져와지게 됩니다.
*   문자 깨짐을 방지하기 위해 UTF-8 BOM 인코딩 사용을 권장합니다.\
    다운로드되는 사용자 정보, 템플릿, 그룹 코드 CSV 파일의 문자 코드는 ‘공유 설정’ > ‘세부기능 설정’ 메뉴의 ‘문자 인코딩’에서 지정되어 있습니다.

    자세한 내용은 [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참고해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**사용자 일괄 등록 화면 표시**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 선택하고 '사용자 일괄 등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (566).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자 일괄 등록 템플릿 다운로드**
{% endhint %}

1. 사용자 일괄 등록 화면의 'CSV 업로드' 설정에서 '샘플 양식' 버튼을 클릭합니다.\
   CSV 파일 템플릿이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (2525).png" alt=""><figcaption></figcaption></figure>

&#x20;  &#x20;

{% hint style="warning" %}
**사용자 추가를 위한 CSV 파일 만들기**
{% endhint %}

1. 다운로드한 템플릿을 편집하여 사용자 추가를 위한 CSV 파일을 만듭니다.

<figure><img src="../../.gitbook/assets/image (568).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="156">항목</th><th width="432">설명</th><th>필수</th></tr></thead><tbody><tr><td>사용자 ID</td><td>로그인할 때 사용자를 식별하는 데 사용되는 사용자 ID를 3~250자 이내로 설정합니다.<br>사용 가능한 문자: 영숫자, 기호(-_@.+#)</td><td>○</td></tr><tr><td>비밀번호</td><td>사용자의 로그인 암호 문자열을 암호 정책에 따라 설정합니다.</td><td> </td></tr><tr><td>이름</td><td>사용자의 표시 이름을 250자 이내로 설정합니다.<br>사용 가능한 문자:<br>UTF-8의 한글, 한자, 영문대소문자, 숫자, 공백, 다국어 문자, 기호 및 이모티콘 등</td><td>○</td></tr><tr><td>이메일 주소</td><td>사용자의 이메일 주소를 250자 이내로 설정합니다.<br>사용 가능한 문자: 영숫자, 기호(-_@.+#)</td><td>○</td></tr><tr><td>전화번호</td><td>사용자의 전화 번호를 50자 이내로 설정합니다.<br>사용 가능한 문자: 숫자, 기호(+-)</td><td> </td></tr><tr><td>언어</td><td><p>다음 언어로 'jpn'(일본어), 'eng'(영어), 'kor'(한국어) 중 하나를 설정합니다.</p><ul><li>사용자 페이지 표시</li><li>사용자에게 보내는 알림 메일</li></ul></td><td> </td></tr><tr><td>할당용량</td><td>My Box의 최대 용량을 계약 계획의 총 저장 용량 내에서 설정합니다.<br>Shared Box의 용량은 포함되지 않습니다.<br>사용 가능한 문자: 1개 이상의 반각 숫자(단위: MB)1024MB는 1GB로 변환됩니다.</td><td>○</td></tr><tr><td>유효기간</td><td>사용자의 만료 날짜를 설정하려면 YYYY-MM-DD 형식으로 날짜를 설정합니다.</td><td> </td></tr><tr><td>상태</td><td>사용자의 상태를 설정합니다.<br>"Y" 또는 입력되지 않은 상태에서 활성화되고 "N"으로 비활성화됩니다.</td><td> </td></tr><tr><td>그룹 코드</td><td>사용자가 속한 그룹의 그룹 코드를 설정합니다.<br>사용자를 여러 그룹에 등록하려면 그룹 코드를 반각 세미콜론(;)으로 구분하여 입력합니다.<br>그룹 코드는 CSV 파일로 그룹 코드 정보를 다운로드하는 방법 에 따라 다운로드할 수 있습니다.</td><td> </td></tr><tr><td>접속 제어</td><td>사용자에게 애플리케이션, 기기 관리, 이중 인증, IP 주소를 기반으로 한 접근 제어를 적용합니다.<br>필요한 보안 정책 > 접속 제어 개별설정 메뉴의 설정 이름을 지정합니다.<br>기본값은 "기본 설정"입니다.</td><td> </td></tr><tr><td>비밀번호 등록 안내 메일 발송</td><td>비밀번호 등록 이메일을 보낼지 여부를 설정합니다.<br>「Y」를 입력하면 패스워드 등록용 메일을 송신합니다.<br>"N" 또는 입력하지 않은 경우 비밀번호 등록 이메일이 전송되지 않습니다.</td><td> </td></tr></tbody></table>



{% hint style="warning" %}
**사용자 추가용 CSV 파일 업로드**
{% endhint %}

1. 사용자 일괄 등록 화면의 'CSV 업로드' 설정에서 사용자 추가를 선택하고 파일 선택 버튼을 클릭하여 생성한 사용자 추가용 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2526).png" alt=""><figcaption></figcaption></figure>



2. '업로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2527).png" alt=""><figcaption></figcaption></figure>



3. CSV 업로드 확인 화면에서 파일명, 입력 행 수, 처리방법을 확인한 후 '바로 신청' 버튼을 클릭합니다.\
   '이메일로 접수 신청서 발행' 버튼을 클릭한 경우 이 매뉴얼의 절차 중 <사용자 추가 최종 요청 제출>에서 최종 신청을 제출하고 사용자를 업로드 합니다.

<figure><img src="../../.gitbook/assets/image (571).png" alt=""><figcaption></figcaption></figure>



4. CSV 파일에 작성한 사용자를 등록합니다. 사용자 추가가 완료되면 "사용자 일괄등록이 완료되었습니다."라는 화면이 표시됩니다. 오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (572).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자 추가 최종 요청 제출**
{% endhint %}

사용자 추가용 CSV 파일 업로드에서 '이메일로 접수 신청서 발행'을 선택한 경우, 신청을 한 계약 관리자 또는 일반 관리자의 이메일 주소로 최종 신청 링크가 포함된 알림 메일이 도착합니다.\
다음 단계에 따라 최종 신청을 제출하고 사용자를 추가합니다.

1. 알림 이메일을 확인하여 '일괄등록 접수하기'의 URL을 클릭합니다.\
   '일괄등록 신청' 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (575).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (576).png" alt=""><figcaption></figcaption></figure>

&#x20;   &#x20;

2. 신청버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (577).png" alt=""><figcaption></figcaption></figure>



3. CSV 파일을 업로드 되고 입력한 사용자가 추가됩니다. \
   사용자 추가가 완료되면 "사용자 일괄등록이 완료되었습니다."라는 화면이 표시됩니다. \
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (578).png" alt=""><figcaption></figcaption></figure>
