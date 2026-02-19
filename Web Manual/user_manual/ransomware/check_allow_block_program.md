---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/ransomware/check_allow_block_program
---

# DirectCloud 드라이브에서 차단/허가된 프로그램을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 기본 기능인 랜섬웨어 대책을 사용하면, 짧은 시간에 여러 번 파일을 변경한 프로그램을 랜섬웨어로 판단하여 자동으로 차단할 수 있습니다.\
이 매뉴얼에서는 랜섬웨어 대책에 의해 차단된 프로그램과 허가된 프로그램을 각각 목록으로 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 기능을 사용하기 위해서는 [랜섬웨어 방지 기능을 사용하는 방법](https://help.directcloud.net/admin_manual/ransomware/enable_ransomware)에서 랜섬웨어 방지가 활성화되어 있어야 합니다.
* 랜섬웨어 대책은 모든 요금제에서 추가 비용 없이 이용할 수 있습니다.
* 랜섬웨어 대책으로 차단되는 대상은 DirectCloud 드라이브에 저장된 파일을 변경한 프로그램만 해당됩니다.
* 프로그램에 의해 파일이 편집된 경우에만 차단되며, 파일을 열기만 한 경우에는 변경으로 판단되지 않습니다.
* 한 번 프로그램이 차단 프로그램으로 등록되면, 동일한 프로그램이 파일을 열기만 해도 변경으로 판단됩니다.
* 디지털 서명이 포함된 프로그램은 이 기능으로 차단할 수 없습니다.
* 관리자 페이지에서도 프로그램 차단 이력을 확인할 수 있습니다.\
  자세한 내용은 [랜섬웨어 방지 기능에 의해 차단된 프로그램의 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/ransomware/blocked_program_history)을 참고해주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**차단된 프로그램 확인**
{% endhint %}

1. PC의 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2496).png" alt=""><figcaption></figcaption></figure>



2. '랜섬웨어 방지' 버튼을 클릭합니다.\
   '랜섬웨어 방지' 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2497).png" alt=""><figcaption></figcaption></figure>



3. '차단된 프로그램' 탭에서 차단된 프로그램을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2500).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="213">항목</th><th>설명</th></tr></thead><tbody><tr><td>대상</td><td>프로그램이 차단될 당시 사용자가 사용하고 있던 OS 정보가 표시됩니다.<br>현재 랜섬웨어 대책을 이용할 수 있는 환경은 Windows용 DirectCloud 드라이브뿐이므로, 이 항목에는 WIN이 표시됩니다.</td></tr><tr><td>프로그램명</td><td>차단된 프로그램의 이름이 표시됩니다.</td></tr><tr><td>경로</td><td>차단된 프로그램의 파일 경로가 표시됩니다.</td></tr><tr><td>해쉬정보</td><td>차단된 프로그램의 해시 값이 표시됩니다.</td></tr><tr><td>날짜</td><td>프로그램이 차단된 날짜와 시간이 표시됩니다.</td></tr><tr><td>허용</td><td>버튼을 클릭하면 허가 프로그램으로 등록할 수 있습니다.<br>자세한 내용은 DirectCloud 드라이브에서 허가 프로그램을 등록/삭제하는 방법을 참고해주시기 바랍니다.</td></tr></tbody></table>



4. 차단된 프로그램을 필터링하여 보고 싶은 경우, 오른쪽 상단의 프로그램명 입력란에 프로그램명에 포함된 문자를 입력한 뒤 검색을 클릭하거나 Enter 키를 누릅니다.



{% hint style="warning" %}
**허용된 프로그램 확인**
{% endhint %}

1. PC의 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2496).png" alt=""><figcaption></figcaption></figure>



2. '랜섬웨어 방지' 버튼을 클릭합니다.\
   '랜섬웨어 방지' 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2497).png" alt=""><figcaption></figcaption></figure>



3. '허용된 프로그램' 탭에서 허용된 프로그램을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2501).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="213">항목</th><th>설명</th></tr></thead><tbody><tr><td>유형</td><td>프로그램이 파일에 접근하기 위한 조건이 표시됩니다.</td></tr><tr><td>대상</td><td>허가 프로그램을 등록할 당시 사용자가 사용하고 있던 기기의 OS 정보가 표시됩니다.<br>현재 랜섬웨어 대책을 이용할 수 있는 환경은 Windows용 DirectCloud 드라이브뿐이므로, 이 항목에는 WIN이 표시됩니다.</td></tr><tr><td>상세정보</td><td><p>등록된 허가 프로그램의 상세 정보가 표시됩니다.</p><ul><li>접근 허가 조건이 해시값 일치인 경우:<br>프로그램 이름과 해시값이 표시됩니다.</li><li>접근 허가 조건이 파일 경로 일치인 경우:<br>프로그램의 파일 경로가 표시됩니다.</li></ul></td></tr><tr><td>등록날짜</td><td>허가 프로그램으로 등록된 날짜와 시간이 표시됩니다.</td></tr><tr><td>삭제</td><td>삭제 버튼을 클릭하면 허가 프로그램 목록에서 삭제할 수 있습니다.<br>자세한 내용은 <a href="https://help.directcloud.net/user_manual/ransomware/register_allow_program">DirectCloud 드라이브에서 허용 프로그램을 등록/삭제하는 방법</a>을 참고해주시기 바랍니다.</td></tr></tbody></table>
