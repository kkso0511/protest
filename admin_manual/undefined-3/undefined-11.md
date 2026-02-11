---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-3/undefined-11
---

# 다수의 사용자 정보를 일괄 삭제하는 방법

### 개요 <a href="#a03" id="a03"></a>

템플릿에 따라 사용자 삭제를 위한 CSV 파일을 만들고 가져오면 한 번에 여러 사용자를 삭제할 수 있습니다.\
이 매뉴얼에서는 사용자 관리 메뉴의 '사용자 일괄 등록'에서 사용자를 삭제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* 삭제 대상 사용자 ID가 등록되어 있지 않은 경우 등록되지 않은 사용자 ID입니다라는 오류가 표시됩니다.\
  사용자를 삭제하려면, 이미 등록된 사용자 ID를 입력한 CSV 파일을 업로드해 주세요.
* 사용자 ID가 일치하면 다른 항목의 내용이 일치하지 않더라도 해당 사용자는 삭제됩니다.
* 가져오기 작업이 진행되는 동안에는 추가로 CSV 가져오기를 요청할 수 없습니다.
* 또한 문자 인코딩이 Shift\_JIS인 CSV 파일이나 텍스트 파일에 X 0213:2004(JIS2004) 규격으로 변경된 옛 한자를 입력하면 저장 시 문자가 깨집니다. 이러한 상태로 CSV 파일이나 텍스트 파일을 가져오면 깨진 문자 그대로 가져와지게 됩니다.
* 문자 깨짐을 방지하기 위해 UTF-8 BOM 인코딩 사용을 권장합니다.\
  내보내기되는 사용자 정보, 템플릿, 그룹 코드 CSV 파일의 문자 인코딩은 환경 설정 > 상세 설정 메뉴의 내보내기 시 문자 인코딩 설정에서 지정할 수 있습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**사용자 일괄 등록 화면 표시**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 선택하고 '사용자 일괄 등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (579).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자 일괄 등록 템플릿 다운로드**
{% endhint %}

1. 사용자 일괄 등록 화면의 'CSV 업로드' 설정에서 '샘플 양식'버튼을 클릭합니다.\
   사용자의 대량 삭제에 사용할 CSV 파일 템플릿이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (2525).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자 삭제를 위한 CSV 파일 만들기**
{% endhint %}

1. 다운로드한 템플릿을 보고 사용자 ID 열에 삭제할 사용자의 사용자 ID를 입력하여 사용자 삭제를 위한 CSV 파일을 만듭니다.

<figure><img src="../../.gitbook/assets/image (1716).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2260).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자 삭제를 위한 CSV 파일 업로드**
{% endhint %}

1. 사용자 일괄 처리 화면의 'CSV 업로드' 설정에서 '사용자 삭제'를 선택하고 파일 선택 버튼을 클릭하여 만든 사용자 삭제를 위한 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1717).png" alt=""><figcaption></figcaption></figure>



2. '업로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1718).png" alt=""><figcaption></figcaption></figure>



3. CSV 업로드 확인 화면에서 파일명, 입력 행 수, 처리방법을 확인한 후 바로신청 버튼을 클릭합니다.\
   '이메일로 접수 신청서 발행' 버튼을 클릭한 경우 이 매뉴얼의 절차 중 <사용자 정보 변경 최종 신청 제출>에서 최종 신청을 제출하고 사용자를 업로드 합니다.

<figure><img src="../../.gitbook/assets/image (1719).png" alt=""><figcaption></figcaption></figure>



4. CSV 파일에 작성한 사용자가 삭제됩니다. \
   삭제가 완료되면 "사용자 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1720).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자 삭제 최종 신청 제출**
{% endhint %}

사용자 삭제용 CSV 파일 업로드에서 '이메일로 접수 신청서 발행'을 선택한 경우, 신청을 한 계약 관리자 또는 일반 관리자의 이메일 주소로 최종 신청 링크가 포함된 알림 메일이 도착합니다.\
다음 단계에 따라 최종 신청을 제출하고 사용자를 삭제합니다.

1. 알림 이메일을 확인하여 '일괄등록 접수하기'의 URL을 클릭합니다.\
   '일괄등록 신청' 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1721).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. '신청' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1722).png" alt=""><figcaption></figcaption></figure>



3. CSV 파일에 작성한 사용자가 삭제됩니다. \
   변경이 완료되면 "사용자 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1723).png" alt=""><figcaption></figcaption></figure>
