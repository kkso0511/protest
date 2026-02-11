---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/undefined-2
---

# 보안문서 판정 기준을 일괄로 등록하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약한 경우, IRM(Information Rights Management)을 이용하여 의도하지 않은 파일 유출을 방지할 수 있습니다.\
DirectCloud-SHIELD IRM에서는 문서 속성으로 보안 문서의 판정 기준을 설정합니다.\
문서 속성은 [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 속성별로 개별 등록할 수 있지만, 이 매뉴얼 에서 설명하는 절차에 따라 문서 속성 추가용 CSV 파일을 생성하여 가져오기를 수행하면 일괄 등록이 가능합니다.\
이 매뉴얼 에서는 'SHIELD' > '설정' 메뉴의 문서 속성 설정에서 보안 문서의 판정 기준을 일괄 등록하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* CSV 파일에 이미 등록되어 있는 문서 속성과 동일한 이름이 포함되어 있는 경우, 문서 속성 설정 정보는 덮어쓰기됩니다. 일괄 등록이 완료되면 완료 화면의 편집 항목 숫자가 증가합니다.
* 문서 속성 정보를 일괄로 삭제할 수는 없습니다.
*   여러 검출 대상을 판정 기준으로 선택하고 AND/OR 조건을 설정하는 경우, 연산자 우선순위가 아니라 왼쪽부터 순차적으로 처리됩니다.

    예: 개인 정보 OR 특정 단어 AND 확장자를 처리하는 경우\
    1번째 처리: 개인 정보 OR 특정 단어\
    2번째 처리: 1번째 처리 결과 AND 확장자
*   상태를 비활성으로 설정하면 라벨이 '보안등급 없음'으로 변경되고, 작업 제한은 해제됩니다.

    한 번 '보안등급 없음' 라벨로 변경되면, 관리자 페이지에서 다시 상태를 활성으로 설정하더라도 '보안등급 없음' 라벨을 원래대로 되돌릴 수는 없습니다.

    단, [파일의 보안등급을 변경하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-7), [사용자 페이지에서 파일의 보안등급을 변경하는 방법](https://help.directcloud.net/user_manual/undefined-3/undefined-4)을 통해 보안등급을 다시 수정하실 수는 있습니다.
* 문자 코드가 Shift\_JIS인 CSV 파일 또는 텍스트 파일에 X 0213:2004(JIS2004) 규격에서 변경된 옛 한자를 입력하는 경우, 저장 시 글자가 깨집니다. 그 상태로 CSV 파일 또는 텍스트 파일을 가져오면, 깨진 상태 그대로 가져오게 됩니다.\
  문자 깨짐을 방지하기 위해 UTF-8 BOM 포함 문자 코드를 사용할 것을 권장합니다.
* 다운로드되는 CSV 파일의 문자 코드는 환경 설정 > 상세 설정 메뉴의 CSV 다운로드 시 문자 코드 설정에서 지정됩니다.\
  자세한 내용은 [다운로드하는CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참고해주시기 바랍니다.

### 절차

{% hint style="info" %}
**문서 속성 일괄 등록용 템플릿을 다운로드합니다.**
{% endhint %}

1. 'SHIELD' > '설정' 메뉴를 선택하고 '속성 정의' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2378).png" alt=""><figcaption></figcaption></figure>

2. 속성 정의에서 '속성 일괄 등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2379).png" alt=""><figcaption></figcaption></figure>

3. 화면을 아래로 스크롤하여 '샘플 양식' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2380).png" alt=""><figcaption></figcaption></figure>

&#x20;     문서 속성 일괄 등록에 사용할 CSV 파일 템플릿이 다운로드됩니다.

{% hint style="info" %}
**문서 속성 일괄 등록용 CSV 파일을 생성합니다.**
{% endhint %}

1. 다운로드한 템플릿을 편집하여 문서 속성 일괄 등록용 CSV 파일을 생성합니다.

<figure><img src="../../.gitbook/assets/image (2381).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="158.60009765625">항목</th><th width="504.5999755859375">내용</th><th>필수</th></tr></thead><tbody><tr><td>속성명</td><td><p>문서 속성명은 50자 이내로 입력합니다.<br></p><p><strong>· 사용 가능한 문자:</strong><br>UTF-8 한자, 히라가나, 영문 대소문자, 숫자, 공백, 다국어 문자, 기호 및 이모지 등<br></p><p><strong>· 사용할 수 없는 문자:</strong><br>반각 &#x3C; > 는 HTML 태그에 사용되는 문자이므로 &#x3C;, >처럼 코드로 변환되어 표시됩니다.<br>또한 HTML의 특수 문자로 사용되는 반각 &#x26; 는 &#x26;로 변환되어 표시됩니다.<br>반각 ￥ 문자는 입력해도 삭제됩니다.</p></td><td>○</td></tr><tr><td>상태</td><td><p>문서 속성의 상태로 Y 또는 N 중 하나를 입력합니다.<br></p><p><strong>·</strong> Y 또는 미입력: 활성<br><strong>·</strong> N: 비활성</p></td><td> </td></tr><tr><td>보안등급</td><td><p>'보안문서 정의' 탭에 입력 되어있는 보안등급 중 하나를 입력해주세요.</p><p>미입력 시 '등급없음'이 적용됩니다.</p></td><td> </td></tr><tr><td>문서 내 개인 정보</td><td><p>문서 내 텍스트에 포함된 개인 정보를 보안 문서의 판정 기준으로 사용할 경우, 대상 개인 정보를 입력합니다.</p><p>입력할 수 있는 개인 정보는 아래와 같습니다.</p><p></p><p>· 주민등록번호</p><p>· 전화번호</p><p>· 이메일주소</p><p>· 국민연금</p><p>· 카드번호</p><p>· 운전면허증번호</p><p>· 이름</p><p>· 주소<br></p><p>여러 항목을 등록할 경우 구분자 ';'를 사용하여 등록해주세요.</p></td><td> </td></tr><tr><td>개인정보 검출조건</td><td><p>문서 내 개인 정보에 여러 개인 정보를 입력한 경우, 보안 문서의 판정 조건을 입력합니다.<br>문서 내 개인 정보가 비어 있거나 하나만 입력된 경우에는 이 항목에 아무것도 입력하지 않습니다.<br></p><p><strong>· OR</strong><br>입력한 개인 정보 중 하나라도 문서 내 텍스트에 포함된 경우<br>미입력 시 자동으로 OR이 적용됩니다.<br></p><p><strong>· AND</strong><br>입력한 개인 정보가 모두 문서 내 텍스트에 포함된 경우</p></td><td> </td></tr><tr><td>개인정보 검출횟수</td><td>문서 내 개인 정보에 입력한 개인 정보가 문서 내 텍스트에 지정한 수 이상 포함된 경우 검색 대상으로 삼으려면 1~99의 반각 숫자를 입력합니다.<br>문서 내 개인 정보가 비어 있는 경우, 이 항목에는 아무것도 입력하지 않습니다.</td><td> </td></tr><tr><td>특정 단어</td><td>문서 내 텍스트 또는 파일명에 포함된 단어를 보안 문서의 판정 기준으로 사용할 경우 단어를 입력합니다.<br>단어는 1개당 30자 이하로 입력해야 합니다.<br>여러 단어를 등록할 경우 반각 세미콜론(;)으로 구분하여 입력합니다.</td><td> </td></tr><tr><td>특정 단어 검출대상</td><td><p>특정 단어를 입력한 경우, 보안 문서의 판정 기준으로 사용할 대상 범위를 지정합니다.<br>특정 단어가 비어 있는 경우, 이 항목에는 아무것도 입력하지 않습니다.<br></p><p><strong>· 본문</strong><br>문서 내 텍스트에 포함된 단어를 보안 문서의 판정 기준으로 사용하는 경우<br></p><p><strong>· 파일명</strong><br>파일명에 포함된 단어를 보안 문서의 판정 기준으로 사용하는 경우<br></p><p>두 항목 모두 지정하려면 반각 세미콜론(;)으로 구분하여 입력합니다.</p></td><td> </td></tr><tr><td>특정 단어 검출조건</td><td><p>특정 단어에 여러 단어를 입력한 경우, 보안 문서의 판정 조건을 입력합니다.<br>특정 단어가 비어 있거나 하나만 입력된 경우에는 이 항목에 아무것도 입력하지 않습니다.<br></p><p><strong>· OR</strong><br>입력한 단어 중 하나라도 문서 내 텍스트 또는 파일명에 포함된 경우<br>미입력 시 자동으로 OR이 적용됩니다.<br></p><p><strong>· AND</strong><br>입력한 단어가 모두 문서 내 텍스트 또는 파일명에 포함된 경우</p></td><td> </td></tr><tr><td>특정 단어 검출횟수</td><td>특정 단어에서 입력한 단어가 문서 내 텍스트에 몇 회 이상 포함되었을 때 보안 문서로 판정할지를 1~99의 반각 숫자로 입력합니다.<br>특정 단어가 비어 있는 경우, 이 항목에는 아무것도 입력하지 않습니다.</td><td> </td></tr><tr><td>확장자</td><td><p>파일의 확장자를 보안 문서의 판정 기준으로 사용할 경우, 아래 확장자를 입력합니다.<br>여러 확장자를 등록하는 경우, 반각 세미콜론(;)으로 구분하여 입력합니다.<br></p><p>· pptx<br>· xlsx<br>· docx<br>· ppt<br>· xls<br>· doc<br>· pdf<br>· txt<br>· dwg</p></td><td> </td></tr><tr><td>판정조건</td><td><p>검출 대상인 문서 내 개인 정보, 특정 단어, 확장자의 설정 상태에 따라 보안 문서의 판정 조건을 입력합니다.<br></p><p><strong>· 3개 항목이 모두 입력된 경우:</strong><br>반각 세미콜론(;)으로 구분하여 아래 조건 패턴 중 하나를 입력합니다.<br>미입력 시 OR;OR이 적용됩니다.<br>-OR;OR<br>-OR;AND<br>-AND;OR<br>-AND;AND<br></p><p><strong>· 2개 항목이 입력된 경우:</strong><br>아래 조건 중 하나를 입력합니다.<br>미입력 시 OR이 적용됩니다.<br>OR<br>AND<br></p><p><strong>· 1개 항목만 입력된 경우:</strong><br>이 항목에는 아무것도 입력하지 않습니다.</p></td><td> </td></tr></tbody></table>

{% hint style="info" %}
**문서 속성 일괄 등록용 CSV 파일을 업로드 합니다.**
{% endhint %}

1. 파일 선택 버튼을 클릭하여 생성한 문서 속성 일괄 등록용 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2382).png" alt=""><figcaption></figcaption></figure>

2. 업로드 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2383).png" alt=""><figcaption></figcaption></figure>

3. 오류 항목에 0이 표시되어 있는 것을 확인한 뒤 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2384).png" alt="" width="563"><figcaption></figcaption></figure>

오류 항목에 1 이상 숫자가 표시된 경우, 이 매뉴얼을 참고하여 CSV 파일을 수정한 뒤 다시 업로드를 진행해주세요.
