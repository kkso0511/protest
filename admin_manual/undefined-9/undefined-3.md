---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-9/undefined-3
---

# 랜섬웨어 방지 기능에서 허용할 프로그램을 등록/삭제하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 기본 기능인 랜섬웨어 방지를 사용하시면, 짧은 시간 안에 여러 차례 파일을 변경한 프로그램을 랜섬웨어로 판단하여 자동으로 차단할 수 있습니다.\
파일 변경을 허용해야 하는 프로그램이 있는 경우, 프로그램이 차단되기 전에 미리 허가 프로그램으로 등록해 둘 수 있습니다.\
이 매뉴얼에서는 허용된 프로그램에 프로그램을 등록하거나, 등록을 삭제하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 랜섬웨어 방지 기능은 모든 플랜에서 추가 요금 없이 이용하실 수 있습니다.
* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '랜섬웨어 방지' 항목에 접근 가능합니다.
* DirectCloud 드라이브의 사용자 페이지에서도 프로그램을 허가 프로그램으로 등록하거나 삭제할 수 있습니다.
* 랜섬웨어 방지에서 차단 대상이 되는 것은 DirectCloud 드라이브에 저장된 파일을 실제로 변경한 프로그램만 해당됩니다.
* macOS용 DirectCloud 드라이브에서는 랜섬웨어 방지 기능을 이용하실 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**'정책적 허용 프로그램' 표시**
{% endhint %}

1. '랜섬웨어 방지' > '설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2160).png" alt=""><figcaption></figcaption></figure>



2. 정책적 허용 프로그램 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2161).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**허용 프로그램 등록**
{% endhint %}

1. 정책적  허용 프로그램에서 추가 버튼을 클릭합니다.\
   '정책적 허용 프로그램'화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2162).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. '파일찾기' 버튼을 클릭하고 정책적 허용 프로그램에 추가할 프로그램을 선택합니다.\
   프로그램이 설정되고 파일에 액세스하기 위한 조건 설정이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2163).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

3. 다음 중 하나를 설정하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2504).png" alt="" width="375"><figcaption></figcaption></figure>

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>해쉬정보</td><td>해시값이 일치할 때 프로그램의 파일 접근을 허가합니다.<br>이 항목을 선택하면 프로그램의 해시값이 자동으로 설정됩니다.</td></tr><tr><td>프로그램 파일 경로</td><td>파일 경로가 일치할 때 프로그램의 파일 접근을 허가합니다.<br>이 항목을 선택한 경우에는 텍스트 박스에 파일의 경로를 입력해야 합니다.</td></tr></tbody></table>



4. 허용 프로그램에 프로그램 정보가 등록되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2165).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="151">항목</th><th>설명</th></tr></thead><tbody><tr><td>유형</td><td>프로그램이 파일에 액세스하는 조건이 표시됩니다.</td></tr><tr><td>상세정보</td><td><p>등록된 권한 프로그램에 대한 자세한 정보가 표시됩니다.</p><ul><li>접근 허용 조건이 해시값 일치인 경우:<br>프로그램 이름과 해시값이 표시됩니다.</li><li>접근 허용 조건이 파일 경로 일치인 경우:<br>프로그램의 파일 경로가 표시됩니다.</li></ul></td></tr><tr><td>대상</td><td>권한 프로그램을 등록할 때 사용자가 사용하던 장치의 OS 정보가 표시됩니다.<br>현재 랜섬웨어 방지 기능은 Windows의 DirectCloud 드라이브에서만 사용할 수 있으므로 이 필드에는 "WIN"이 표시됩니다.</td></tr><tr><td>날짜</td><td>프로그램이 권한 프로그램에 등록된 날짜와 시간이 표시됩니다.</td></tr><tr><td>동작</td><td>권한 프로그램에 등록된 프로그램을 삭제하는 버튼이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**정책적 허용 프로그램 삭제**
{% endhint %}

1. 정책적 허용 프로그램에서 삭제할 프로그램의 삭제 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2166).png" alt=""><figcaption></figcaption></figure>



2. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2167).png" alt=""><figcaption></figcaption></figure>



3. '허용 프로그램'에서 삭제한 프로그램의 표시가 사라졌는지 확인합니다.
