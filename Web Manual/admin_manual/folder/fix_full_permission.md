---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/folder/fix_full_permission
---

# 폴더 생성 시 모든 사용자의 접근 권한을 <전체권한>으로 고정하는 방법

### 개요 <a href="#a03" id="a03"></a>

'Shared Box' 메뉴에서는 모든 사용자 및 Guest의 접근 권한이 '<전체권한>'으로 고정되는 폴더 유형을 생성할 수 있습니다.\
접근 권한을 설정하지 않고 DirectCloud의 주요 기능을 사용할 수 있으므로, 공개 범위를 제한하지 않고 간편하게 정보를 공유하고자 하는 경우에 유용합니다.\
이 매뉴얼에서는 'Shared Box' 메뉴에서 폴더를 생성할 때 모든 사용자 및 Guest의 접근 권한을 <전체권한>으로 고정하도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '공유 설정'에 접근 가능합니다.
* '공유 대상'이 '모든 사용자'인 폴더를 생성할 수 있는 것은 제1계층만 해당됩니다.
* '공유 대상'이 '모든 사용자'인 폴더에서는 사용자·그룹을 지정한 접근 권한 설정을 할 수 없으므로, '그룹/사용자'의 '접근 권한 설정' 버튼은 표시되지 않습니다.
* '공유 대상'이 '모든 사용자'인 폴더에서는 모든 사용자가 <전체권한>으로 고정되므로, <마스터>의 '접근 권한 설정' 버튼은 표시되지 않습니다.
* '공유 대상'이 '모든 사용자'인 폴더에서는 Guest의 '접근 권한 설정' 버튼은 표시되지만, 설정 가능한 접근 권한은 <전체권한>으로 고정됩니다.
* '공유 대상'이 '모든 사용자'인 폴더의 속성은 '특정 사용자'의 폴더 속성과 동일하게 사용할 수 있습니다.
* 폴더의 공유 사용자를 '모든 사용자'에서 '특정 사용자'로 변경할 수 있으나, 한 번 변경하면 '모든 사용자' 폴더로 되돌릴 수 없습니다.
* '모든 사용자' 폴더를 생성한 후 '특정 사용자가 '모든 사용자'인 폴더 생성' 설정을 비활성화하더라도, 이미 생성된 폴더는 '특정 사용자'로 변경되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**'공유 대상'이 '모든 사용자'인 폴더 생성을 활성화**
{% endhint %}

1. '공유 설정' > 'Shared Box 관리' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>



2. '모든 사용자 폴더 생성' 항목에서 '사용'에 체크합니다.\
   설정은 즉시 저장됩니다.

<figure><img src="../../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**'공유 대상'이 '모든 사용자'인 폴더 생성**
{% endhint %}

1. [관리자 페이지에서 폴더를 생성하는 방법](https://help.directcloud.net/admin_manual/folder/create_folder)에 따라 제1계층의 '새폴더 생성' 화면을 표시합니다.

<figure><img src="../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>



2. 새 폴더의 이름을 입력하고 '공유대상'에서 '모든 사용자'를 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="217.5">공유 대상</th><th>설명</th></tr></thead><tbody><tr><td>모든 사용자</td><td>폴더를 생성하는 시점에 모든 사용자에게 &#x3C;전체권한>의 접근 권한이 부여됩니다.<br>사용자·그룹을 지정하여 접근 권한을 부여·변경·삭제할 수 없습니다.</td></tr><tr><td>지정한 사용자</td><td>사용자·그룹을 지정하여 접근 권한을 부여·변경·삭제할 수 있습니다.</td></tr></tbody></table>



3. 생성된 폴더를 선택하고 '공유 대상'이 '모든 사용자'로 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**'공유 대상'을 '특정 사용자'로 변경**
{% endhint %}

1. '공유 대상' 설정에서 '수정' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>



2. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>



3. '공유 대상'이 '특정 사용자'로 변경되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>
