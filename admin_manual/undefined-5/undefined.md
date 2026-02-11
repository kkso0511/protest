---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-5/undefined
---

# 폴더 경로에 드라이브 문자를 할당하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '공유 설정' > '맞춤형 설정' 메뉴의 드라이브 문자 설정에서, DirectCloud 드라이브의 폴더 경로에 할당할 드라이브 문자를 지정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정' 메뉴를 사용할 수 있습니다.
* 2023년 6월 8일(목) 업데이트로 '공유 설정' > '상세 설정'의 'DirectCloud 드라이브의 드라이브 문자 고정'은\
  '공유 설정' > '맞춤형 설정'의 '드라이브 문자 설정'으로 변경되었습니다.
* 'DirectCloud 드라이브의 드라이브 문자 고정'에서 지정되어 있던 드라이브 문자는 '드라이브 문자 설정'의 '/DirectCloud/' 드라이브 문자로 계승되었습니다.
* 루트 폴더 경로인 '/DirectCloud/'의 드라이브 문자는 기본적으로 '자동 할당'으로 설정되어 있습니다.
* 루트 폴더 경로인 '/DirectCloud/'는 변경할 수 없습니다.
* 루트 폴더 이외의 폴더 경로는 '드라이브 문자 설정'에서 변경할 수 있습니다.
* '할당 대상 폴더 선택' 화면에서 폴더를 선택할 때 입력한 폴더 경로가 220자를 초과하면 '폴더 경로에 입력 가능한 문자 수의 상한을 초과했습니다.'라고 표시됩니다.
* '드라이브 문자 할당 설정'에서 관리되고 있는 폴더 경로에 포함된 폴더 이름이 변경되거나 폴더가 이동된 경우, 폴더 경로도 자동으로 변환됩니다.
* '드라이브 문자 할당 설정'에서 관리되고 있는 폴더 경로에 포함된 폴더가 삭제된 경우, '드라이브 문자 할당 설정'의 '드라이브 경로' 아래에 '삭제된 폴더'라고 표시됩니다.
* 폴더 경로에는 'My Box', 'Connect', 'DLP' 폴더를 지정할 수 없습니다.
* 드라이브 문자는 A부터 Z까지(C 제외) 총 25자 중에서 선택할 수 있습니다.
* 본 매뉴얼의 절차에 따라 드라이브 문자를 지정한 경우, 사용자 페이지에서는 [DirectCloud 드라이브에서 폴더 경로에 할당된 드라이브 문자를 확인하는 방법](https://help.directcloud.net/user_manual/undefined-13/directcloud-3)의 절차로 드라이브 문자를 변경할 수 없게 됩니다.
* 사용자가 DirectCloud 드라이브에 로그인한 후 본 매뉴얼의 절차로 설정이 변경된 경우, 사용자가 애플리케이션을 재시작했을 때 변경 사항이 반영됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**폴더 경로에 할당된 드라이브 문자 확인**
{% endhint %}

1. '공유 설정' > '맞춤형 설정' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2041).png" alt=""><figcaption></figcaption></figure>



2. '드라이브 문자 설정'에서 드라이브 문자가 할당된 폴더 경로 목록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2043).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="190">항목</th><th>설명</th></tr></thead><tbody><tr><td>드라이브 문자</td><td><p>폴더 경로에 할당할 드라이브 문자를 다음 중에서 선택합니다.</p><ul><li>자동 할당:<br>사용자가 DirectCloud 드라이브에 로그인할 때 자동으로 드라이브 문자가 할당됩니다.</li><li>"A"~"Z"("C" 제외):<br>25자 중 하나를 선택합니다.<br>사용자가 DirectCloud 드라이브에 로그인하면 여기에 지정된 고정 드라이브 문자가 할당됩니다.</li></ul></td></tr><tr><td>연결 위치</td><td>드라이브 문자가 할당된 폴더 경로가 표시됩니다.<br>폴더 경로는 최대 220자로 설정해야 합니다.<br>폴더 경로의 문자 수에는 폴더 구분 기호도 포함되지만 드라이브 문자, 루트 폴더 이름(DirectCloud) 및 "Shared Box"문자 수는 포함되지 않습니다.</td></tr><tr><td>표시 명칭</td><td>Windows 탐색기에 표시되는 이름을 설정합니다.<br>표시 가능한 문자 수 상한: 150자</td></tr><tr><td>동작</td><td><ul><li>기본값:<br>루트 폴더의 '/DirectCloud/'에 표시됩니다. 수동으로 루트 폴더 설정을 삭제할 수 없습니다.</li><li>휴지통 버튼:<br>클릭하면 할당된 드라이브 문자를 삭제할 수 있습니다.<br>자세한 내용은 할당된 드라이브 문자의 설정 삭제를 참조하십시오.</li></ul></td></tr></tbody></table>



{% hint style="warning" %}
**폴더 경로에 드라이브 문자 할당**
{% endhint %}

1. '드라이브 문자 설정'에서 '추가'버튼을 클릭합니다.\
   드라이브 문자 할당 설정 행이 추가됩니다.

<figure><img src="../../.gitbook/assets/image (2044).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. 드라이브 문자 열에서 폴더 경로에 할당할 드라이브 문자를 선택합니다.\
   이미 사용 중인 드라이브 문자는 선택할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (2045).png" alt=""><figcaption></figcaption></figure>



3. 할당할 폴더 경로를 선택합니다(클릭)을 클릭합니다.\
   할당 대상 폴더를 선택하는 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2046).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

4. 드라이브 문자를 할당할 폴더를 선택하고 확인 버튼을 클릭합니다.\
   선택한 폴더의 폴더 경로가 설정됩니다.

<figure><img src="../../.gitbook/assets/image (2047).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

5. 필요한 경우 표시 이름을 변경합니다.

<figure><img src="../../.gitbook/assets/image (2048).png" alt=""><figcaption></figcaption></figure>



6. 저장 버튼을 클릭합니다.\
   드라이브 문자 할당 설정이 저장됩니다.

<figure><img src="../../.gitbook/assets/image (2049).png" alt=""><figcaption></figcaption></figure>

&#x20;   &#x20;

{% hint style="info" %}
**할당된 드라이브 문자의 설정 삭제**
{% endhint %}

1. 드라이브 문자 할당 설정에서 삭제할 할당 설정의 작업 열에 있는 휴지통 버튼을 클릭합니다.\
   클릭한 드라이브 문자의 할당 설정 표시가 사라집니다.

<figure><img src="../../.gitbook/assets/image (2050).png" alt=""><figcaption></figcaption></figure>

&#x20;   &#x20;

2. 저장 버튼을 클릭합니다.\
   드라이브 문자 할당 설정이 저장됩니다.

<figure><img src="../../.gitbook/assets/image (2051).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

{% hint style="warning" %}
**Directcloud 드라이브에서 확인**
{% endhint %}

1. DirectCloud 드라이브에 로그인하고 Windows 탐색기에 선택한 드라이브 문자가 할당되어 있는지 확인합니다.
