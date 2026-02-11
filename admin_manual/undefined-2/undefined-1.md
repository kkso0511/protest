---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-2/undefined-1
---

# 그룹을 일괄 등록하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 사용자 관리 메뉴에서 사용자가 속한 그룹을 일괄 등록하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '계정 관리' 항목에 접근할 수 있습니다.
*   1단계 그룹부터 한 번에 등록할 수 있습니다.

    예를 들어, 1단계의 ‘A 그룹’ 폴더 아래에 2단계의 ‘B 그룹’ 폴더를 생성하고 싶은 경우,\
    ‘A 그룹/B 그룹’이라고 입력하면 상위 그룹인 A 그룹과 하위 그룹인 B 그룹이 동시에 생성됩니다.
*   ‘계정 관리’ 메뉴에 표시되는 각 그룹은 상·하위 관계를 유지하고 있지만,\
    접근 권한을 부여할 때는 각각을 독립된 그룹으로 취급해야 합니다.

    따라서 폴더의 접근 권한을 상위 단계 그룹에 부여하더라도,\
    그 하위 단계에 있는 그룹까지 자동으로 적용되도록 설정할 수는 없습니다.

    각 그룹별로 개별적으로 접근 권한을 부여해 주세요.
* 이미 동일한 이름의 그룹이 생성되어 있는 경우에는 해당 처리가 건너뛰어지고, 다음 작업으로 진행됩니다.
*   만들 수 있는 그룹 수의 사양은 다음과 같습니다.

    | 만들 수 있는 그룹의 계층 구조     | 50 계층까지 |
    | --------------------- | ------- |
    | 1계층에 작성할 수 있는 그룹 수    | 3,844까지 |
    | 단일 프로세스로 만들 수 있는 그룹 수 | 100까지   |
*   그룹 이름에 사용할 수 있는 문자와 사용할 수 없는 문자는 다음과 같습니다.

    * 사용 가능한 문자\
      UTF-8의 한글,  한자, 영문대소문자, 숫자, 공백, 다국어 문자, 기호 및 이모티콘 등
    * 사용할 수 없는 문자\
      /\\:\*?"<> |

    문자 코드는 UTF-8 BOM 포함을 사용해 주세요
*   템플릿으로 다운로드되는 텍스트 파일의 문자 코드는 ‘공유 설정’ > ‘세부 기능 설정’ 메뉴에 있는 ‘문자 인코딩’에서 지정되어 있습니다.

    자세한 내용은 [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참고해 주세요.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**일괄 등록 템플릿을 사용하여 일괄 등록하기**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 선택하고 그룹 일괄등록 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (484).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 ‘일괄 등록 양식’ 설정을 표시한 뒤, 등록하려는 그룹 이름을 1단계부터 입력합니다.\
   하위 그룹을 함께 등록하려는 경우에는 ‘/’(반각 슬래시)로 구분하여 입력합니다.

<figure><img src="../../.gitbook/assets/image (486).png" alt=""><figcaption></figcaption></figure>



3. 일괄 등록 그룹의 입력이 끝나면 '템플릿등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (487).png" alt=""><figcaption></figcaption></figure>



4.  그룹 일괄 등록 완료 화면에서 오류 번호가 ‘0’인지 확인한 뒤, ‘확인’ 버튼을 클릭합니다.

    오류 번호가 ‘1’ 이상인 경우에는 제한·보충 사항을 충분히 읽은 다음, 다시 2단계를 실행해 주세요.

<figure><img src="../../.gitbook/assets/image (488).png" alt=""><figcaption></figcaption></figure>

그룹이 일괄 등록됩니다.

<figure><img src="../../.gitbook/assets/image (489).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**텍스트 파일로 그룹 일괄 등록하기**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 선택하고 '그룹 일괄등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (490).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 'TXT 파일을 이용한 등록'을 표시한 다음 '샘플 양식' 버튼을 클릭합니다.\
   그룹 일괄 등록 샘플 양식의 텍스트 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (491).png" alt=""><figcaption></figcaption></figure>





3. 다운로드한 텍스트 파일에 등록하려는 그룹 이름을 1단계부터 입력합니다.\
   하위 그룹을 함께 등록하려는 경우에는 ‘/’(반각 슬래시)로 구분하여 입력합니다.

<figure><img src="../../.gitbook/assets/image (2517).png" alt=""><figcaption></figcaption></figure>



4. 파일 선택 버튼 클릭하고 3단계에서 작성한 텍스트 파일을 선택하고 템플릿등록 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (493).png" alt=""><figcaption></figcaption></figure>



5.  그룹 일괄 등록 완료 화면에서 오류 번호가 ‘0’인지 확인한 뒤, ‘확인’ 버튼을 클릭합니다.

    오류 번호가 ‘1’ 이상인 경우에는 제한·보충 사항을 충분히 읽은 다음, 다시 3\~4단계를 실행해 주세요.

<figure><img src="../../.gitbook/assets/image (494).png" alt=""><figcaption></figcaption></figure>

그룹이 일괄 등록됩니다.

<figure><img src="../../.gitbook/assets/image (495).png" alt=""><figcaption></figcaption></figure>
