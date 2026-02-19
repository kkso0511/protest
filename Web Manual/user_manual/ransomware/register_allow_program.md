---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/ransomware/register_allow_program
---

# DirectCloud 드라이브에서 허용 프로그램을 등록/제거하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 기본 기능인 랜섬웨어 대책을 사용하면, 짧은 시간에 여러 번 파일을 변경한 프로그램을 랜섬웨어로 판단하여 자동으로 차단할 수 있습니다.\
파일 변경을 허용해야 하는 프로그램이 있는 경우, 해당 프로그램이 차단되기 전에 미리 허가 프로그램으로 등록해 둘 수 있습니다.\
이 매뉴얼에서는 DirectCloud 드라이브에서 프로그램을 허용된 프로그램에 등록하거나 등록을 삭제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 기능을 사용하기 위해서는 [랜섬웨어 방지 기능을 사용하는 방법](https://help.directcloud.net/admin_manual/ransomware/enable_ransomware)에서 랜섬웨어 방지가 활성화되어 있어야 합니다.
* 랜섬웨어 대책은 모든 요금제에서 추가 비용 없이 이용할 수 있습니다.
* 랜섬웨어 대책으로 차단되는 대상은 DirectCloud 드라이브에 저장된 파일을 변경한 프로그램만 해당됩니다. 프로그램에 의해 파일이 편집된 경우에만 차단되며, 파일을 열기만 한 경우에는 변경으로 판단되지 않습니다.
* 한 번 프로그램이 차단 프로그램으로 등록되면, 동일한 프로그램이 파일을 열기만 해도 변경으로 판단됩니다.
* 디지털 서명이 포함된 프로그램은 이 기능으로 차단할 수 없습니다.
* 관리자 페이지에서도 프로그램 차단 이력을 확인할 수 있습니다.\
  자세한 내용은 [랜섬웨어 방지 기능에 의해 차단된 프로그램의 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/ransomware/blocked_program_history)을 참고해주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**랜섬웨어 방지 화면을 표시**
{% endhint %}

1. PC의 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2496).png" alt=""><figcaption></figcaption></figure>



2. '랜섬웨어 방지' 버튼을 클릭합니다.\
   '랜섬웨어 방지' 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2497).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**허용된 프로그램 탭에서 허용 프로그램 등록**
{% endhint %}

1. 랜섬웨어 방지 화면에서 '허용된 프로그램' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2501).png" alt=""><figcaption></figcaption></figure>



2. '추가' 버튼을 클릭합니다.\
   허용 프로그램 등록 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2502).png" alt=""><figcaption></figcaption></figure>



3. '파일찾기' 버튼을 클릭하고 허용 프로그램에 추가할 프로그램을 선택한 다음 '열기' 버튼을 클릭합니다. 프로그램이 설정되고 "허용 프로그램에 등록"화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2503).png" alt=""><figcaption></figcaption></figure>



4. 프로그램이 파일에 액세스하기 위한 조건으로 다음 중 하나를 선택하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2504).png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>해쉬정보</td><td>해시값이 일치할 때 프로그램의 파일 접근을 허가합니다.<br>이 항목을 선택하면 프로그램의 해시값이 자동으로 설정됩니다.</td></tr><tr><td>프로그램 파일 경로</td><td>파일 경로가 일치할 때 프로그램의 파일 접근을 허가합니다.<br>이 항목을 선택한 경우에는 텍스트 박스에 파일의 경로를 입력해야 합니다.</td></tr></tbody></table>

'허용된 프로그램'에 프로그램의 정보가 등록됩니다.



{% hint style="warning" %}
**차단된 프로그램 탭에서 허용 프로그램 등록**
{% endhint %}

1. 랜섬웨어 방지 화면에서 차단 프로그램 탭을 클릭합니다.\
   차단된 프로그램이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2500).png" alt=""><figcaption></figcaption></figure>



2. 허용 프로그램으로 등록하려는 차단 프로그램의 "허용" 열에 있는 버튼을 클릭합니다.\
   '허용 프로그램에 등록'화면이 표시됩니다.



3. 프로그램이 파일에 접근하기 위한 조건으로 아래 항목 중 하나를 선택한 뒤 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2504).png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="200">항목</th><th>설명</th></tr></thead><tbody><tr><td>해쉬정보</td><td>해시값이 일치할 때 프로그램의 파일 접근을 허가합니다.<br>이 항목을 선택하면 프로그램의 해시값이 자동으로 설정됩니다.</td></tr><tr><td>프로그램 파일 경로</td><td>파일 경로가 일치할 때 프로그램의 파일 접근을 허가합니다.<br>이 항목을 선택한 경우에는 텍스트 박스에 파일의 경로를 입력해야 합니다.</td></tr></tbody></table>

'허용된 프로그램'에 프로그램의 정보가 등록됩니다.



{% hint style="warning" %}
**허용 프로그램 삭제**
{% endhint %}

1. 허용된 프로그램 탭에서 삭제하려는 프로그램의 삭제 열에 있는 버튼을 클릭합니다.
2. 허용된 프로그램에서 삭제된 프로그램이 목록에서 사라졌는지 확인합니다.
