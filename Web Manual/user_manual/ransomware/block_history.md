---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/ransomware/block_history
---

# DirectCloud 드라이브에서 프로그램이 차단된 내역을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 기본 기능인 랜섬웨어 방지 기능을 사용하면, 짧은 시간에 여러 번 파일을 변경하는 프로그램을 랜섬웨어로 판단하여 자동으로 차단할 수 있습니다.\
아래 매뉴얼의 절차에 따라 프로그램이 차단되면 '차단된 프로그램'에 자동으로 등록되며, 프로그램 차단 이력에 로그가 기록됩니다.

* [랜섬웨어 방지 기능을 통해 보호하려는 파일의 확장자를 지정하는 방법](https://help.directcloud.net/admin_manual/ransomware/file_extension)
* [랜섬웨어 방지 기능에서 프로그램이 차단되기까지의 변경 횟수를 설정하는](https://help.directcloud.net/admin_manual/ransomware/change_count)

이 매뉴얼 에서는 랜섬웨어 대책에 의해 프로그램이 차단된 이력을 DirectCloud 드라이브에서 확인하는 방법에 대해 설명합니다.

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
**프로그램 차단 내역 보기**
{% endhint %}

1. PC의 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2496).png" alt=""><figcaption></figcaption></figure>



2. '랜섬웨어 방지' 버튼을 클릭합니다.\
   '랜섬웨어 방지' 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2497).png" alt=""><figcaption></figcaption></figure>



3. 프로그램 차단 기록 탭에서 프로그램이 차단된 기록을 확인하십시오.

<figure><img src="../../.gitbook/assets/image (2498).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="167">항목</th><th>설명</th></tr></thead><tbody><tr><td>컴퓨터명</td><td>프로그램이 차단될 당시 사용자가 사용하고 있던 기기의 컴퓨터 이름이 표시됩니다.</td></tr><tr><td>프로그램명</td><td>차단된 프로그램의 이름이 표시됩니다.</td></tr><tr><td>경로</td><td>차단된 프로그램의 파일 경로가 표시됩니다.</td></tr><tr><td>날짜</td><td>프로그램이 차단된 날짜와 시간이 표시됩니다.</td></tr><tr><td>사유</td><td><p>프로그램이 차단된 이유가 표시됩니다.</p><ul><li>파일 변조 시도:<br>프로그램에 의한 파일 변경 횟수가 랜섬웨어 대책에서 설정한 차단 기준 횟수 이상이 되어 프로그램이 차단된 경우에 표시됩니다.</li><li>차단 등록된 프로그램:<br>프로그램이 차단 프로그램에 등록되어 있어 차단된 경우에 표시됩니다.</li></ul></td></tr><tr><td>상세 표시 버튼                                 </td><td>클릭하면 차단 이유에 따라 자세한 정보가 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**프로그램 차단 내역에 대해 자세히 알아보기**
{% endhint %}

1. 차단 내역에서 차단 사유가 '파일 변경 작업 감지'로 표시된 프로그램의 상세 표시 버튼을 클릭합니다.\
   차단된 프로그램의 해시값과 서명 정보 외에도, 해당 프로그램에 의해 변경된 파일의 이름이 표시됩니다.



{% hint style="warning" %}
**프로그램 차단 내역을 필터링하여 표시하기**
{% endhint %}

프로그램 차단 내역 화면에서는 프로그램 차단 내역을 기간, 차단 사유, 프로그램명으로 필터링하여 표시할 수 있습니다.

<table><thead><tr><th width="156">항목</th><th>설명</th></tr></thead><tbody><tr><td>기간</td><td>계약 시작부터 현재까지 차단된 프로그램의 기록을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>사유</td><td><p>클릭하여 드롭다운 목록을 보고 좁히고 보려는 차단 이유로 다음 중 하나를 선택합니다.</p><ul><li>파일 변조 시도:<br>프로그램에 의한 파일 변경 횟수가 랜섬웨어 대책에서 설정한 차단 기준 횟수 이상이 되어 프로그램이 차단된 경우에 표시됩니다.</li><li>차단 등록된 프로그램:<br>프로그램이 차단 프로그램에 등록되어 있어 차단된 경우에 표시됩니다.</li></ul></td></tr><tr><td>프로그램 이름                          </td><td>프로그램 차단 내역을 프로그램명으로 좁히는 경우에 입력합니다.</td></tr></tbody></table>
