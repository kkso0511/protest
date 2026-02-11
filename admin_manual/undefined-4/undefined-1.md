---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-4/undefined-1
---

# 관리자 페이지에서 폴더 이름을 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 관리 페이지의 'Shared Box' 메뉴에서 폴더 이름을 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 본 매뉴얼에서는 '공유 설정' > 'Shared Box' 메뉴의 조작 방법에 대해 기재하고 있으나, 'Shared Box' 메뉴 이외의 폴더에 대해서도 동일한 절차로 생성할 수 있습니다.
* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '공유 설정'에 접근 가능합니다.
* 제1계층의 폴더 이름을 변경할 수 있는 접근 권한은 <마스터>만 가능합니다.
* 제2계층 이후의 폴더 이름을 변경할 수 있는 접근 권한은 <마스터>, <전체권한>, <편집자>입니다.
* 폴더를 일괄로 등록하는 방법의 절차에서는 폴더 이름을 일괄로 변경할 수 없습니다.
*   루트 폴더의 표시명인 'Shared Box', 'Connect', 'DLP', 'Warm Storage'는 변경할 수 없습니다.

    루트 폴더의 표시명인 'Shared Box'는 변경할 수 없습니다.
*   폴더는 노드값이라는 고유한 값으로 관리됩니다.\
    이 값은 DirectCloud의 관리자 API에서 폴더를 지정할 때 사용됩니다.

    예를 들어 'Shared Box'의 루트 폴더에는 '1{2'라는 값이 할당되어 있으며, 하위 계층에 폴더가 생성될 때마다 3문자씩 노드값이 추가됩니다. 아래에 예를 제시합니다.

    제1계층: 1{2Sh8\
    제2계층: 1{2Sh89ZT\
    제3계층: 1{2Sh89ZT9jK
* 폴더 이름의 끝에 반각 마침표(.) 또는 공백 문자가 포함되어 있는 경우, Windows의 제한으로 인해 DirectCloud 드라이브에서는 폴더를 사용할 수 없습니다.\
  본 매뉴얼의 절차에 따라 Web 브라우저에서 폴더 이름의 끝에 상기 문자열이 포함되지 않도록 수정하면 DirectCloud 드라이브에서 폴더를 사용할 수 있게 됩니다.
* 'DirectCloud-CONNECT'를 사용할 수 있는 경우, 관리 페이지의 '공유 설정' > 'Connect 관리' 메뉴에서 폴더 이름을 변경할 수 있습니다.
* 'DirectCloud-SHIELD DLP'를 계약한 경우, 관리 페이지의 '공유 설정' > 'DLP 관리' 메뉴에서 폴더 이름을 변경할 수 있습니다.
* 'Warm Storage'를 계약한 경우, 관리 페이지의 '공유 설정' > 'Warm Storage 관리' 메뉴에서 폴더 이름을 변경할 수 있습니다.
* Warm Storage에서는 업로드 시 알림 메일이 전송되지 않기 때문에, '공유 설정' > 'Warm Storage 관리'에서 제1계층의 폴더 이름을 변경할 때 표시되는 '폴더 이름 변경' 화면에는 '알림 설정'이 표시되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '공유 설정' > 'Shared Box' 관리 메뉴를 선택하고 폴더 이름을 변경할 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1835).png" alt=""><figcaption></figcaption></figure>



2.  아래 중 하나의 방법으로 '폴더 이름 변경' 화면을 표시합니다.

    ❶ 왼쪽 상단에 있는 '수정' 버튼을 클릭\
    ❷ '공유 설정'의 '폴더 이름' 오른쪽에 있는 '폴더 수정' 버튼을 클릭\
    ❸ 폴더 트리에서 이름을 변경하려는 폴더를 오른쪽 클릭한 후, 표시된 메뉴에서 '수정'을 클릭

<figure><img src="../../.gitbook/assets/image (1836).png" alt=""><figcaption></figcaption></figure>



3. '폴더명 수정' 화면에서 폴더 이름 입력란에 변경할 폴더 이름을 입력하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1837).png" alt=""><figcaption></figcaption></figure>



4. 폴더 이름이 변경되었는지 확인합니다.
