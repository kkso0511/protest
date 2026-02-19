---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_share/add_to_address_book
---

# 메일 수신처 정보를 주소록에 등록하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 '공유 링크', '파일첨부 메일발송', '업로드 요청', 'Guest 초대', 'Connect User 초대'의 생성 화면에서 송신처를 설정할 때, 아래의 주소록에서 메일 주소를 선택할 수 있습니다.

* 개인 주소록
* 회사 주소록
* 생성한 주소록

이 매뉴얼에서는 각 주소록에 발신 대상을 등록하는 방법과, 등록된 이메일 주소를 수정하거나 삭제하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 사용자가 개인 주소록과 회사 주소록을 사용하려면, 관리자가 관리자 페이지에서 ‘회사 주소록 공개’ 설정을 ‘사용함’을 선택해야 합니다.
* Guest가 개인 주소록과 회사 주소록을 사용하려면, 위의 설정에 더해 ‘Guest' 의 '기능 예외’ 설정의 ‘주소록’ 항목에서 ‘회사주소록/개인주소록 모두 사용함’을 선택해야 합니다.
* 개인 주소록에는 다음 절차에 따라 대상에 설정된 이메일 주소가 자동으로 추가됩니다.\
  새로 이메일 주소를 등록할 수도 있습니다.
* 회사 주소록에는 관리자 페이지의 '계정관리' > '사용자' 메뉴에 등록된 사용자의 이메일 주소가 자동으로 추가됩니다. 새로 이메일 주소를 등록할 수 없습니다.
* 개인 주소록과 회사 주소록 외에도 용도에 맞는 이메일 주소 그룹을 '내 주소록'으로 만들 수 있습니다.
* 개인 주소록과 내 주소록에는 최대 60,000개의 주소를 등록할 수 있습니다.
* 내 주소록의 이름은 100자 이내로 설정해야 합니다.
* 주소록의 '소속'은 DirectCloud 그룹 이름과 다릅니다.\
  회사 이름과 같은 임의의 소속 정보를 추가할 수 있습니다.
* 회사 주소록, 내 주소록 대상 정보를 CSV 파일로 일괄 내보낼 수 없습니다.
* CSV 파일을 사용하여 대상 정보를 회사 주소록, 내 주소록에 일괄 등록할 수 없습니다.
* 다른 외부 프로그램과 주소록을 연동시킬 수 없습니다.
* 주소록에 등록된 대상 정보를 재정렬할 수 없습니다.
* 개인 주소록과 템플릿을 내보낼 때의 문자 인코딩은 관리자 페이지에서 EUC-KR 또는 UTF-8 BOM로 설정할수 있습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**대상 정보를 주소록에 추가**
{% endhint %}

**\[주소록 메뉴 표시]**

1. 주소록 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1135).png" alt=""><figcaption></figcaption></figure>

주소록 화면이 표시됩니다.\
주소록 화면에는 다음 내용이 표시됩니다.

| 항목     | 설명                                                                                                       |
| ------ | -------------------------------------------------------------------------------------------------------- |
| 이름     | 이름이 표시됩니다. 설정되지 않은 경우에는 빈칸으로 표시됩니다.                                                                      |
| 이메일 주소 | 이메일 주소가 표시됩니다. 커서를 올리면 버튼이 나타나며, 이 버튼을 클릭하면 이메일 주소를 클립보드에 복사할 수 있습니다.                                    |
| 전화번호   | 전화번호가 표시됩니다. 설정되지 않은 경우에는 빈칸으로 표시됩니다.                                                                    |
| 소속     | 소속 정보가 표시됩니다. 설정되지 않은 경우에는 빈칸으로 표시됩니다.                                                                   |
| 구분     | <p>다음 중 하나의 주소록 구분이 표시됩니다. ‘내 주소록’에 등록된 주소는 ‘개인 주소록’으로 구분됩니다.</p><ul><li>회사 주소록</li><li>개인 주소록</li></ul> |



**\[새 주소록 만들기]**

이 매뉴얼에서는 주소록을 만드는 방법에 대해 설명합니다.

1. 상단에 표시된 주소록을 클릭한 다음 표시된 목록에서 "주소그룹 설정" 을클릭합니다.

<figure><img src="../../.gitbook/assets/image (1136).png" alt=""><figcaption></figcaption></figure>



2. 만들려는 주소록의 이름을 입력하고  추가 버튼을 클릭합니다.\
   주소록이 저장됩니다.

<figure><img src="../../.gitbook/assets/image (1137).png" alt=""><figcaption></figcaption></figure>



3. 닫기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1138).png" alt=""><figcaption></figcaption></figure>



4. 만든 주소록이 주소록 목록에 추가되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1139).png" alt=""><figcaption></figcaption></figure>



**\[대상 정보 추가]**

1. 상단에 표시된 주소록을 클릭한 다음 표시된 목록에서 대상 정보를 추가할 개인 주소록 또는 생성한 주소록을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1140).png" alt=""><figcaption></figcaption></figure>



2. '새연락처' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1141).png" alt=""><figcaption></figcaption></figure>



3. 등록하고자 하는 목적지 정보를 입력하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1142).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="158">항목</th><th width="502.79998779296875">설명</th><th>필수여부</th></tr></thead><tbody><tr><td>주소그룹</td><td>현재 설정되어 있는 수신처 정보를 등록하는 내 주소록의 이름이 표시됩니다.<br>내 주소가 반각 하이픈(-)인 경우 드롭다운 목록에서 내 주소록을 선택하여 개인 주소록 외에 선택한 내 주소록에 대상 정보를 등록합니다. 수 있습니다.</td><td> </td></tr><tr><td>이메일 주소</td><td>등록하려는 이메일 주소를 250자 이내로 입력합니다.<br>최상위 도메인(TLD)에 설정할 수 있는 최대 문자 수는 20자입니다.</td><td>〇</td></tr><tr><td>이름</td><td>이름을 250자 이내로 입력합니다.</td><td> </td></tr><tr><td>전화번호</td><td>전화 번호를 50자 이내로 입력합니다.</td><td> </td></tr><tr><td>소속</td><td>소속을 50자 이내로 입력합니다.</td><td> </td></tr><tr><td>메모</td><td>이메일 주소에 대한 정보를 1,000자 이내로 입력합니다.</td><td> </td></tr></tbody></table>



4. 주소록에 대상 정보가 추가되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1143).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**주소록에 등록된 수신처 정보 변경**
{% endhint %}

1. 주소록 메뉴에서 다음 방법 중 하나를 사용하여 주소 변경 화면을 표시합니다.

❶ 정보를 변경하고자 하는 주소를 체크하고 상단 메뉴에서 변경 아이콘을 클릭

<figure><img src="../../.gitbook/assets/image (1144).png" alt=""><figcaption></figcaption></figure>

❷ 정보를 변경할 주소를 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 편집을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1147).png" alt=""><figcaption></figcaption></figure>

❸ 정보를 변경하고 싶은 주소의 우측에 있는 ▼ 버튼을 클릭하고, 표시되는 메뉴로부터 「편집집」을 클릭

<figure><img src="../../.gitbook/assets/image (1146).png" alt=""><figcaption></figcaption></figure>



2. 대상 정보를 변경하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1149).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th>항목</th><th width="521">설명</th><th>필수 여부</th></tr></thead><tbody><tr><td>내 주소록</td><td>현재 설정되어 있는 수신처 정보를 등록하는 내 주소록의 이름이 표시됩니다.<br>내 주소가 반각 하이픈(-)인 경우 드롭다운 목록에서 내 주소록을 선택하여 개인 주소록 외에 선택한 내 주소록에 대상 정보를 등록합니다. 수 있습니다.</td><td> </td></tr><tr><td>이메일 주소</td><td>등록하려는 이메일 주소를 250자 이내로 입력합니다.<br>최상위 도메인(TLD)에 설정할 수 있는 최대 문자 수는 20자입니다.</td><td>〇</td></tr><tr><td>이름</td><td>이름을 250자 이내로 입력합니다.</td><td> </td></tr><tr><td>전화번호</td><td>전화 번호를 50자 이내로 입력합니다.</td><td> </td></tr><tr><td>소속</td><td>소속을 50자 이내로 입력합니다.</td><td> </td></tr><tr><td>메모</td><td>이메일 주소에 대한 정보를 1,000자 이내로 입력합니다.</td><td> </td></tr></tbody></table>



3. 대상 정보가 변경되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1150).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**주소록에 등록된 수신인 정보 삭제**
{% endhint %}

1. 주소록 메뉴에서 다음 방법 중 하나를 사용하여 주소를 삭제합니다.

❶  삭제할 주소를 체크하고 상단 메뉴에서 '삭제' 아이콘을 클릭

<figure><img src="../../.gitbook/assets/image (1151).png" alt=""><figcaption></figcaption></figure>

❷  삭제할 주소를 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 "삭제"를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1152).png" alt=""><figcaption></figcaption></figure>

❸  삭제할 주소의 오른쪽에 있는 ▼ 버튼을 클릭하고 표시된 메뉴에서 '삭제'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1153).png" alt=""><figcaption></figcaption></figure>

삭제 확인 화면이 표시됩니다.



2. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1154).png" alt=""><figcaption></figcaption></figure>

주소가 삭제됩니다.

<figure><img src="../../.gitbook/assets/image (1155).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**개인 주소록의 대상 정보를 CSV 파일로 내보내기**
{% endhint %}

1. 주소록 메뉴에서 오른쪽 상단의 '현재 주소록 CSV 다운로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1156).png" alt=""><figcaption></figcaption></figure>

주소록의 대상 정보 목록이 CSV 파일로 다운로드됩니다.



2. 다운로드된 CSV 파일을 확인합니다.



{% hint style="warning" %}
**CSV 파일을 사용하여 대상 정보를 개인 주소록에 일괄 등록**
{% endhint %}

**\[CSV 일괄등록 화면 표시]**

1. 주소록 화면에서 오른쪽 상단의 'CSV 일괄등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1157).png" alt=""><figcaption></figcaption></figure>

CSV 일괄등록 화면이 표시됩니다.



**\[주소 일괄 등록용 템플릿 다운로드]**

1. CSV 일괄등록 화면에서 '샘플 CSV 다운로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1158).png" alt=""><figcaption></figcaption></figure>

주소 일괄 등록에 사용할 CSV 파일 템플릿이 다운로드됩니다.



**\[주소 일괄 등록을 ​​위한 CSV 파일 만들기]**

1. 다운로드한 템플릿을 편집하여 주소 일괄 등록을 ​​위한 CSV 파일을 만듭니다.\
   새로 추가할 대상 정보와 정보를 변경하려는 대상 정보를 입력할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1159).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th>항목</th><th width="500.7999267578125">설명</th><th>필수 여부</th></tr></thead><tbody><tr><td>이메일 주소</td><td>등록하려는 이메일 주소를 250자 이내로 입력합니다.<br>최상위 도메인(TLD)에 설정할 수 있는 최대 문자 수는 20자입니다.</td><td>〇</td></tr><tr><td>이름</td><td>이름을 250자 이내로 입력합니다.</td><td> </td></tr><tr><td>전화번호</td><td>전화 번호를 50자 이내로 입력합니다.</td><td> </td></tr><tr><td>소속</td><td>소속을 50자 이내로 입력합니다.</td><td> </td></tr><tr><td>메모</td><td>이메일 주소에 대한 정보를 1,000자 이내로 입력합니다.</td><td> </td></tr></tbody></table>



**\[주소 일괄 등록을 ​​위한 CSV 파일 가져오기]**

1. CSV 일괄등록 화면에서 '파일 선택' 버튼을 클릭하고 작성한 사용자 추가용 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1160).png" alt=""><figcaption></figcaption></figure>

2. 등록버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1161).png" alt=""><figcaption></figcaption></figure>

CSV 파일에 나열된 대상 정보를 가져옵니다.



3. CSV 일괄등록 결과를 확인하고 닫기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1162).png" alt=""><figcaption></figcaption></figure>

| 항목   | 설명                                                                 |
| ---- | ------------------------------------------------------------------ |
| 전체   | 가져온 대상 정보의 수가 표시됩니다.                                               |
| 신규   | 등록된 대상 정보의 수가 표시됩니다.                                               |
| 업데이트 | 변경된 대상 정보의 수가 표시됩니다.                                               |
| 오류   | CSV 파일을 작성하는 데 문제가 있기 때문에 오류가 발생하여 등록 또는 변경할 수 없는 대상 정보의 수가 표시됩니다. |
