---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/group/move_group
---

# 그룹을 이동하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud 관리 페이지에서는 화면에서 그룹을 선택해 다른 그룹 아래로 바로 이동시키는 것은 불가능합니다.\
그룹을 이동하려면 먼저 이동할 대상 그룹을 생성한 후, 사용자 정보를 해당 그룹으로 옮겨야 합니다.\
이 매뉴얼에서는 ‘사용자 일괄 처리’ 기능을 활용하여 그룹을 이동하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '계정 관리' 항목에 접근할 수 있습니다.
*   그룹은 두 자리로 구성된 그룹 코드로 관리됩니다. 그룹을 생성할 때는 ‘상위 그룹의 2자리 그룹 코드 + 새로 부여되는 본인의 2자리 그룹 코드’가 함께 등록됩니다.&#x20;

    예를 들어, ‘회사명’ 그룹의 그룹 코드가 ‘AA’인 경우 ‘회사명’ 바로 아래에 첫 번째 그룹을 생성하면 ‘AAAA’가 등록되고, 두 번째 그룹을 생성하면 ‘AAAB’가 등록됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

이 절차에서는 ‘A부’ 바로 아래에 있는 ‘A과’를 ‘B부’ 바로 아래로 이동하는 경우를 예로 들어 설명합니다.

{% hint style="warning" %}
**이동 대상 그룹 만들기**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (506).png" alt=""><figcaption></figcaption></figure>



2. 이동할 대상인 ‘B부’ 그룹을 마우스 오른쪽 버튼으로 클릭한 뒤, 표시되는 메뉴에서 ‘그룹 추가’를 클릭합니다.\
   또는 이동할 대상인 ‘B부’ 그룹을 선택한 후, 상단에 있는 ‘그룹 추가’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure>



3. ‘그룹이름'에 ‘A과’를 입력한 뒤, ‘사용 권한 추가’에 ‘보안 정책’ > ‘사용 권한’ 메뉴에서 생성해 둔 이름을 선택하고, 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**이동할 사용자 정보의 CSV 파일 편집**
{% endhint %}

1. [그룹 코드 정보를 CSV 파일로 다운로드하는 방법](https://help.directcloud.net/admin_manual/group/group_code_csv_download)의 단계에 따라 그룹 코드 정보를 CSV 파일로 다운로드합니다.



2. 다운로드한 그룹 코드 정보 CSV 파일을 열어, 이동 전인 ‘A부/A과’의 그룹 코드와 이동 후인 ‘B부/A과’의 그룹 코드를 확인합니다.

<figure><img src="../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>



3. [다수의 사용자를 일괄 등록하는 방법](https://help.directcloud.net/admin_manual/user/bulk_register) 의 단계에 따라 사용자 정보를 CSV 파일로 다운로드합니다.



4. 사용자 정보 CSV 파일을 열어, ‘A부A과’의 그룹 코드를 ‘B부A과’의 그룹 코드로 수정합니다.

<figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>

<p align="center">⬇️</p>

<figure><img src="../../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>



5.  이동 대상인 ‘B부A과’의 그룹 코드 행을 제외한 나머지 그룹 코드 행은 이번 절차에서는 편집 대상이 아니므로 모두 삭제합니다.

    아래는 불필요한 행을 삭제한 이후의 상태입니다.

<figure><img src="../../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**이동할 그룹으로 사용자 정보 가져오기**
{% endhint %}

편집한 사용자 정보의 CSV 파일을 사용하여 사용자 정보를 'B부' 바로 아래의 'A과'로 가져옵니다.

1. 사용자 일괄 처리 등록에서 'CSV 업로드'의 '사용자 수정'을 선택하고 '파일 선택' 버튼을 클릭하여 편집한 사용자 정보의 CSV 파일을 선택합니다.

<figure><img src="../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

2. 업로드 버튼을 클릭하여 CSV 파일을 가져옵니다.



{% hint style="warning" %}
**기존그룹 삭제**
{% endhint %}

이동 전 기존 그룹인 ‘A부’ 바로 아래에 있는 ‘A과’를 삭제합니다.

1. 삭제할 그룹을 마우스 오른쪽 버튼으로 클릭한 뒤, 표시되는 메뉴에서 ‘삭제’를 클릭합니다.\
   또는 삭제하려는 그룹을 선택한 후, 상단에 있는 ‘삭제’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>



2. 그룹 삭제 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>
