---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/workflow/bulk_delete
---

# 워크플로우를 일괄 삭제하는 방법

### 개요 <a href="#a03" id="a03"></a>

워크플로우를 사용하면 사용자가 다음 작업을 수행할 때 결재자가 승인할 수 있도록 설정할 수 있습니다.

* 다운로드
* 링크전송
* 파일첨부 메일발송
* 업로드

워크플로우의 신청자로 지정된 사용자가 대상 기능을 이용하기 위한 승인 신청을 하고, 워크플로우의 결재자로 지정된 사용자에 의해 승인됨으로써, 비로소 조작이 가능해지는 구조입니다.\
템플릿에 따라 워크플로우 삭제용 CSV 파일을 생성하여 업로드하면, 여러 개의 워크플로우를 일괄로 삭제할 수 있습니다.\
이 매뉴얼에서는, '워크플로우' > '설정' 메뉴의 '워크플로우 일괄 등록'에서 워크플로우 설정을 삭제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '워크플로우' 항목을 사용할 수 있습니다.
* 워크플로우를 이용하려면 [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)의 절차에 따라, '워크플로우 설정'에서 '사용'이 선택되어 있어야 합니다.
* [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)에서 워크플로우가 활성화되어 있더라도, [특정 폴더에서 워크플로우를 활성화하 방법](https://help.directcloud.net/admin_manual/folder/enable_workflow)에서 '워크플로우' 설정이 '사용 안함'으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
* 워크플로우 삭제용 CSV 파일에는, 삭제하고 싶은 워크플로우의 행만 기재해 주시기 바랍니다.\
  워크플로우 ID가 기재되어 있으면 해당 워크플로우가 삭제되므로, 주의가 필요합니다.
* 워크플로우 삭제용 CSV 파일에 필요한 정보는, 워크플로우 ID만 해당됩니다.\
  워크플로우 ID 외의 항목에 입력할 수도 있지만, 입력한 내용은 사용되지 않습니다.
*   문자 코드가 Shift\_JIS인 CSV 파일 또는 텍스트 파일에 X 0213:2004(통칭 JIS2004) 규격에서 변경된 구자체 문자를 입력하면, 저장 시 문자가 깨집니다. 그 상태에서 CSV 파일이나 텍스트 파일을 가져오면, 깨진 문자가 그대로 가져와집니다.

    문자 깨짐을 방지하기 위해 문자 코드로 UTF-8 BOM 포함을 사용할 것을 권장합니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**워크플로우 일괄 등록 화면 표시**
{% endhint %}

1. '워크플로우' > '설정' 메뉴를 선택하고 생성된 '워크플로우 관리' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2076).png" alt=""><figcaption></figcaption></figure>



2. '결재선 일괄 등록' 버튼을 클릭합니다.\
   결재선 일괄 등록 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2077).png" alt=""><figcaption></figcaption></figure>

&#x20;   &#x20;

{% hint style="warning" %}
**워크플로우 삭제를 위한 CSV 파일 만들기**
{% endhint %}

현재 등록된 워크플로우를 CSV 형식으로 다운로드하여 워크플로우 삭제를 위한 CSV 파일로 사용할 수 있습니다.\
다운로드에 대한 자세한 내용은 [워크플로우 결재선을 CSV 파일로 다운로드 하는 방법](https://help.directcloud.net/admin_manual/undefined-7/csv)을 참조하세요.

1. 다운로드한 워크플로우의 CSV 파일을 확인해 워크플로우 삭제를 위한 CSV 파일을 만듭니다.\
   **결재선 ID를 체크하여 일치하는 결재선을 삭제하니 주의하시기 바랍니다.**\
   **워크플로우 삭제용 CSV 파일에는 삭제할 워크플로우의 행만 포함하십시오.**

<figure><img src="../../.gitbook/assets/image (2540).png" alt=""><figcaption></figcaption></figure>

<p align="center"> ⬇️</p>

<figure><img src="../../.gitbook/assets/image (2541).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**워크플로우 삭제를 위한 CSV 파일 업로드**
{% endhint %}

1. 워크플로우 일괄 등록 화면의 'CSV 업로드' 설정에서 '결재선 삭제'를 선택하고 파일 선택 버튼을 클릭하여, 생성한 워크플로우 삭제 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2079).png" alt=""><figcaption></figcaption></figure>



2. 업로드 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2080).png" alt=""><figcaption></figcaption></figure>



3. CSV 업로드 확인 화면에서 '파일명, 입력 행 수, 처리방법'을 확인한 후 바로 신청 버튼을 클릭합니다. \
   '이메일로 접수 신청서 발행' 버튼을 클릭한 경우 이 매뉴얼의 절차 중 '**워크플로우 삭제 최종 신청서 제출'** 단계에서 최종 신청서를 제출하고 워크플로우를 업로드 합니다.

<figure><img src="../../.gitbook/assets/image (2081).png" alt=""><figcaption></figcaption></figure>



4. CSV 파일에 입력된 워크플로우를 등록하여 결재선을 삭제합니다.\
   워크플로우 추가가 완료되면 "결재선 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2085).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**워크플로우 삭제 최종 신청서 제출**
{% endhint %}

워크플로우 삭제를 위한 'CSV 파일 업로드' 화면에서 '이메일로 접수신청서 발행'을 선택한 경우, 계약 담당자 또는 일반 관리자의 이메일 주소로 최종 요청 링크가 발송됩니다.\
아래 절차에 따라 최종 신청서를 전송하여 워크플로우를 삭제합니다.

1. 이메일을 열고 '일괄 등록 접수하기' URL을 클릭합니다.\
   일괄등록 신청 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2082).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. '신청' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2083).png" alt=""><figcaption></figcaption></figure>



3. CSV 파일에 입력된 워크플로우를 등록하여 결재선을 삭제합니다.\
   워크플로우 추가가 완료되면 "결재선 일괄등록이 완료되었습니다."라는 화면이 표시됩니다.\
   오류가 없는지 확인하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2084).png" alt=""><figcaption></figcaption></figure>
