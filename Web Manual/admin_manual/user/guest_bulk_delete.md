---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/guest_bulk_delete
---

# Guest 정보를 일괄 삭제하는 방법

### 개요 <a href="#a03" id="a03"></a>

템플릿에 맞춰 Guest 삭제용 CSV 파일을 작성한 후 업로드하면, 여러 명의 Guest를 한 번에 삭제할 수 있습니다.이 매뉴얼에서는 ‘Guest' 관리 메뉴의 ‘Guest 일괄 등록’에서 Guest를 삭제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
*   삭제 대상 사용자 ID가 등록되어 있지 않은 경우에는 ‘등록되지 않은 사용자 ID입니다.’라는 오류가 표시됩니다.

    Guest를 삭제하려면, 이미 등록되어 있는 사용자 ID를 입력한 CSV 파일을 업로드해 주시기 바랍니다.\
    사용자 ID가 일치하는 Guest는 다른 항목의 설정 내용이 일치하지 않더라도 삭제됩니다.
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
**Guest 삭제용 CSV 파일 만들기**
{% endhint %}

1. 다운로드한 템플릿을 열어 ‘사용자 ID’ 열에 **삭제하려는 Guest의 사용자 ID를 입력**한 후, Guest 삭제용 CSV 파일을 작성합니다.

<figure><img src="../../.gitbook/assets/image (78).png" alt=""><figcaption></figcaption></figure>

<p align="center">⬇️</p>

<figure><img src="../../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Guest 삭제용 CSV 파일 업로드**
{% endhint %}

1. ‘Guest 일괄 등록’ 화면의 ‘CSV 업로드’ 설정에서 ‘Guest 삭제’를 선택한 후, ‘파일 선택’ 버튼을 클릭하여 작성한 Guest 삭제용 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>



2. '업로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (82).png" alt=""><figcaption></figcaption></figure>



3.  CSV 업로드 확인 화면에서 ‘파일명’, ‘등록 행 수’, ‘처리 유형’을 확인한 후 ‘바로 신청’ 버튼을 클릭합니다.

    ‘이메일로 접수 신청서 발행’ 버튼을 클릭한 경우에는 이 매뉴얼의 \<Guest 삭제 최종 신청 제출>의 절차에 따라 최종신청을 전송한 후 Guest를 업로드해 주시기 바랍니다.

<figure><img src="../../.gitbook/assets/image (1791).png" alt=""><figcaption></figcaption></figure>



4. CSV 파일에 기재된 Guest가 삭제됩니다. \
   Guest 삭제가 완료되면 "Guest 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1795).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Guest 삭제 최종 신청 제출**
{% endhint %}

Guest 삭제용 CSV 파일 업로드에서 ‘이메일로 접수 신청서 발행’을 선택한 경우에는, 업로드 요청을 생성한 계약 담당 관리자 또는 일반 관리자의 이메일 주소로 최종 신청용 링크가 포함된 안내 메일이 발송됩니다.\
아래 절차에 따라 최종 신청을 전송하고 Guest를 삭제해 주시기 바랍니다.

1. 안내 메일을 열고 ‘일괄등록 접수하기' URL을 클릭합니다.\
   '일괄등록 신청'화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1792).png" alt=""><figcaption></figcaption></figure>



2. '신청' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1793).png" alt=""><figcaption></figcaption></figure>



3. CSV 파일이 업로드되며, 파일에 기재된 Guest가 삭제됩니다. \
   Guest 삭제가 완료되면 "Guest 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1794).png" alt=""><figcaption></figcaption></figure>
