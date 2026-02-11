---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-4/less-than-greater-than-1
---

# 사용자에게 <마스터> 권한을 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 <마스터> 권한은 조작할 수 있는 범위에 따라 <마스터>, <마스터1>, <마스터2>의 접근 레벨로 구분됩니다.\
이 매뉴얼에서는 폴더를 선택하여 마스터 권한 중 하나를 사용자에게 부여하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* 각 마스터 권한에는 아래와 같은 차이가 있습니다.\
  자세한 내용은 [접근 레벨의 종류와 Web 브라우저에서 가능한 작업](https://help.directcloud.net/user_manual/undefined-5/web)을 참고해 주십시오.
  * 마스터\
    제1계층의 폴더에 대한 작업(이름 변경 및 삭제)에 더해,\
    제2계층 이후의 폴더에 대한 모든 작업과 파일에 관한 모든 작업이 가능합니다.
  * 마스터1\
    마스터 권한에서 '폴더 속성 설정'을 제외한 작업이 가능합니다.
  * 마스터2\
    마스터 권한에서 '접근 권한 설정'을 제외한 작업이 가능합니다.
* <마스터>는 제1계층의 폴더에 대해 설정합니다. 설정 내용은 하위 폴더로 상속됩니다.
* 사용자에게 제1계층의 폴더를 생성할 수 있는 권한을 부여하는 방법의 절차에 따라 제1계층의 폴더를 생성한 사용자는 자동으로 해당 폴더의 <마스터>가 됩니다.
* <마스터>, <마스터1>, <마스터2> 이외의 접근 레벨이 부여된 사용자에게 <마스터>, <마스터1>, <마스터2> 권한을 설정하면, 변경 전의 접근 레벨은 자동으로 삭제됩니다.
* <마스터>, <마스터1>, <마스터2> 권한을 삭제하면, 다시 변경 전의 접근 레벨이 부여됩니다.
* <마스터>, <마스터1>, <마스터2> 권한이 부여된 사용자에게는 그 외의 접근 레벨을 설정할 수 없습니다.
* Guest에게 <마스터> 권한을 부여할 수 없습니다.
* 'DirectCloud-CONNECT'를 사용할 수 있는 경우, 관리 페이지에 '공유 설정' > 'Connect 관리' 메뉴가 표시됩니다.
* 'DirectCloud-SHIELD DLP'를 계약한 경우, 관리 페이지에 '공유 설정' > 'DLP 관리' 메뉴가 표시됩니다.
* 'Warm Storage'를 계약한 경우, 관리 페이지에 '공유 설정' > 'Warm Storage 관리' 메뉴가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="info" %}
**Shared Box 폴더를 지정하여 사용자에게 <마스터> 권한 부여**
{% endhint %}

1. '공유 설정' > 'Shared Box 관리' 메뉴를 선택하고 <마스터>를 설정하려는 1계층 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1973).png" alt=""><figcaption></figcaption></figure>



2. '구성원 관리'에서 '마스터' 오른쪽에 표시되는 '마스터 관리' 버튼을 클릭합니다.\
   마스터 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1974).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. 마스터 권한을 부여하려는 사용자를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1975).png" alt=""><figcaption></figcaption></figure>

이때 사용자의 이름이나 ID로 좁혀 검색할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1976).png" alt=""><figcaption></figcaption></figure>



4. 추가 버튼을 클릭합니다. 선택한 사용자가 오른쪽 영역으로 이동합니다.

<figure><img src="../../.gitbook/assets/image (1977).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

5. 마스터 권한 사용자의 만료 날짜를 설정하려면 체크박스를 선택하고 날짜를 클릭한 다음 표시된 캘린더에서 날짜를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1978).png" alt=""><figcaption></figcaption></figure>



6. 드롭다운 목록에서 구성할 마스터 권한의유형에 따라 항목을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1979).png" alt=""><figcaption></figcaption></figure>

| 마스터 유형       | 항목                   |
| ------------ | -------------------- |
| 전체 기능 제공     | 모든 기능 허용을 선택합니다.     |
| 권한 관리 기능만 제공 | 권한 관리만 허용을 선택합니다.    |
| 폴더 환경 설정만 제공 | 폴더 속성 설정만 허용을 선택합니다. |



7. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1980).png" alt=""><figcaption></figcaption></figure>



8. '구성원 관리'의 '마스터' 아이콘에 추가한 마스터의 수가 추가되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1981).png" alt=""><figcaption></figcaption></figure>
