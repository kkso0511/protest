---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-4/undefined-9
---

# 폴더를 일괄 등록하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 전용 폼에 입력하거나 텍스트 파일을 가져오는 방식으로 폴더를 일괄 등록할 수 있습니다.\
이 매뉴얼에서는 폴더를 일괄 등록하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '공유 설정' 메뉴를 사용할 수 있습니다.
* 폴더 이름을 일괄로 수정할 수 없습니다.
* 폴더를 일괄로 삭제할 수 없습니다.
* [폴더 생성 시 모든 사용자의 접근 권한을 <전체권한>으로 고정하는 방법](https://help.directcloud.net/admin_manual/undefined-4/less-than-greater-than)에 따라 생성한, '공유 대상'이 '모든 사용자'인 폴더를 폴더 경로에 포함하여 등록하면 오류가 발생합니다. 이 경우 아래 중 하나의 방법으로 대응해 주십시오.
  * 대상 사용자가 '지정한 사용자'인 폴더만 포함된 폴더 경로를 등록합니다.
  * 폴더 경로를 신규로 등록합니다.
*   만들 수 있는 폴더 수의 사양은 다음과 같습니다.

    | 만들 수 있는 폴더의 계층 구조              | 60까지                                                                                                                                                        |
    | ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
    | 하나의 폴더에 저장할 수 있는 폴더와 파일 수(이론값) | <ul><li>폴더: 238,328까지</li><li>파일: 238,328까지</li></ul><p><strong>참고:</strong><br>많은 양의 폴더와 파일을 저장하면 성능이 저하되므로 1 폴더 내의 폴더와 파일의 합계가 2,000개 이내에 맞도록 해야 합니다.</p> |
    | 한 번의 처리로 만들 수 있는 폴더 수          | 100까지                                                                                                                                                       |
* 폴더와 파일 이름, 전체 경로의 문자 수는 1바이트(byte) 단위가 아니며 한글을 구분하지 않고 한 문자로 계산됩니다.
* 아래에 해당하는 190자 이내의 폴더 이름을 등록할 수 있습니다.
  * 사용 가능한 문자:\
    UTF-8의 한자, 한글, 영문 대소문자, 숫자, 공백, 다국어 문자, 기호 및 이모티콘 등
  * 사용할 수 없는 문자:\
    \ / : \* ? “ < > |
* 폴더의 전체 경로는 260자 이내로 설정해야 합니다.\
  전체 경로의 문자 수에는 폴더 구분 기호, 드라이브 문자, 루트 폴더 이름(DirectCloud) 및 "Shared Box" 문자도 포함됩니다.
* Mac 버전의 DirectCloud 드라이브를 사용 중인 경우, 아래와 같은 상한이 있으므로 주의해 주십시오.
  * 폴더 이름: 255바이트
  * 폴더의 전체 경로: 1,024바이트
* 폴더는 노드 값이라는 고유한 값으로 관리됩니다. 이 값은 DirectCloud의 관리자 API에서 폴더를 지정하는 데 사용됩니다.\
  예를 들어, "공유"의 루트 폴더에는 "1{2" 값이 할당되며 하위 계층 구조에 폴더가 생성될 때마다 3자씩 노드 값이 추가됩니다.\
  예를 들면 다음과 같습니다.\
  　제1 계층: 1{2Sh8\
  　제2 계층: 1{2Sh89ZT\
  　제3 계층: 1{2Sh89ZT9jK\
  일괄 등록에서는, 이미 같은 이름(노드값)의 폴더가 있었을 경우, 스킵 처리됩니다.
* 'Connect', 'DLP', '문서 관리', 'Warm Storage', 'Cold Storage'의 폴더도 'Shared Box' 폴더와 마찬가지로 고유한 노드값으로 관리됩니다. 일괄 등록 시 이미 동일한 이름(노드값)의 폴더가 존재하는 경우, 해당 항목은 스킵 처리됩니다.
* 문자 코드가 'Shift\_JIS'인 CSV 파일 또는 텍스트 파일에 X 0213:2004(통칭 JIS2004) 규격으로 변경된 구자체 문자를 입력하면 저장 시 문자가 깨집니다. 이 상태로 CSV 파일 또는 텍스트 파일을 가져오면 문자가 깨진 상태로 가져와집니다. 문자 깨짐 방지를 위해 문자 코드는 UTF-8 BOM 포함 사용을 권장합니다.
* 템플릿으로 내보내는 텍스트 파일의 문자 코드는 '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정됩니다. 자세한 내용은 [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv) 참조하십시오.
* HTML 파일을 사용하여 폴더를 일괄 등록할 수 없습니다.
* 계약 플랜이 엔터프라이즈이며 DirectCloud의 무료 옵션인 'DirectCloud-CONNECT'를 사용할 수 있는 경우,\
  관리 페이지의 '공유 설정' > 'Connect 관리' 메뉴에서 폴더를 일괄 등록할 수 있습니다.
* 'DirectCloud-SHIELD DLP'를 계약한 경우, 관리 페이지의 '공유 설정' > 'DLP 관리' 메뉴에서 폴더를 일괄 등록할 수 있습니다.
* Warm Storage를 사용할 수 있는경우, 관리 페이지의 '공유 설정' > 'Warm Storage 관리' 메뉴에서 폴더를 일괄 등록할 수 있습니다.
* 'Cold Storage'를 계약한 경우, 관리 페이지의 '공유 설정' > 'Cold Storage 관리' 메뉴에서 폴더를 일괄 등록할 수 있습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Shared Box 폴더 일괄 등록**
{% endhint %}

**\[템플릿을 사용해 등록]**

1. '공유 설정' > 'Shared Box 관리' 메뉴를 선택하고 '공유폴더 일괄 등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1861).png" alt=""><figcaption></figcaption></figure>



2. '공유폴더 일괄 등록' 설정이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1878).png" alt=""><figcaption></figcaption></figure>



3. 화면을 아래로 스크롤하여 '일괄 등록 템플릿'을 표시하고 등록하려는 폴더의 폴더 경로를 한 줄에 하나씩 입력한 다음 '템플릿등록' 버튼을 클릭합니다.\
   폴더의 경로는 "\\"로 구분하여 입력합니다.

<figure><img src="../../.gitbook/assets/image (1879).png" alt=""><figcaption></figcaption></figure>



4. "폴더 일괄 등록을 완료하였습니다."라는 메시지가 표시됩니다. \
   확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1880).png" alt=""><figcaption></figcaption></figure>



5. 폴더 트리에서 폴더가 등록되어 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1881).png" alt=""><figcaption></figcaption></figure>



**\[텍스트 파일로 등록]**

1. '공유 설정' > 'Shared Box 관리' 메뉴를 선택하고 '폴더 일괄 등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1882).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 'TXT 파일을 이용한 등록'을 표시한 다음 '샘플 양식' 버튼을 클릭합니다.\
   텍스트 형식의 템플릿 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1883).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. 템플릿 파일에 따라 등록할 폴더의 폴더 경로를 한 줄에 하나씩 입력합니다.\
   2단계에서 다운로드한 템플릿 파일에 입력할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1884).png" alt=""><figcaption></figcaption></figure>



4. 'TXT 파일을 이용한 등록'에서 '파일 선택' 버튼을 클릭하고 3단계에서 만든 텍스트 파일을 선택한 후, '탬플릿 등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1885).png" alt=""><figcaption></figcaption></figure>



5. "폴더 일괄 등록을 완료하였습니다."라는 메시지가 표시됩니다.\
   확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1886).png" alt=""><figcaption></figcaption></figure>



6. 폴더 트리에서 폴더가 등록되어 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1887).png" alt=""><figcaption></figcaption></figure>
