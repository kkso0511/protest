---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/account_settings/d_network_diagnosis
---

# DirectCloud 드라이브의 설정 화면에서 PC와 네트워크 환경을 진단하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud 드라이브의 동작과 관련된 문제가 발생했을 때, 사용 중인 PC와 네트워크 정보를 수집하여 DirectCloud로 전송하면 원인 분석과 신속한 문제 해결에 도움이 될 수 있습니다.\
이 매뉴얼에서는 DirectCloud 드라이브의 설정 화면에서 환경 진단을 수행하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* **‘**&#x44;irectCloud 드라이브 접속환경 진단’의 진단 결과는 1개월간 보관됩니다.\
  최근 7일 이내에 ‘접속환경 진단’을 실행한 적이 있는 경우, ‘접속환경 진단’ 화면에 그 진단 결과가 표시됩니다.
* ‘접속환경 진단’을 이용하려면 아래 도메인에 대한 통신을 허용하도록 설정해야 합니다.\
  \- sp.directcloud.jp

***

### 절차

{% hint style="warning" %}
**DirectCloud 드라이브 접속환경 진단 실행하기**
{% endhint %}

1. DirectCloud 드라이브에 로그인합니다.



2. 작업 표시줄의 트레이 영역에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브의 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2247).png" alt=""><figcaption></figcaption></figure>



3. 설정 화면의 오른쪽 상단에 있는 '⁝' 버튼을 클릭한 후, 표시된 메뉴에서 '접속환경 진단'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2249).png" alt=""><figcaption></figcaption></figure>



4. 환경 진단을 시작하려면 수집된 PC 및 네트워크 정보를 DirectCloud로 전송해야 합니다.\
   수집되는 정보, 수집 목적, 보관 및 이용 기간에 동의하는 경우에는 ‘위의 내용에 동의합니다’에 체크한 후 ‘진단 시작’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2250).png" alt="" width="563"><figcaption></figcaption></figure>

&#x20;     환경 진단이 시작되며 진행 상태가 표시됩니다.\
&#x20;     환경 진단에는 몇 분 정도 소요됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-10 162245.png" alt="" width="563"><figcaption></figcaption></figure>

&#x20;     환경 진단이 완료되면 진단 결과가 표시됩니다.\
&#x20;     또한 진단 결과는 로그 폴더에 저장됩니다.



5. ‘DirectCloud에 진단결과 보내기’ 버튼을 클릭합니다.

{% hint style="info" %}
**NOTE**\
오른쪽 상단의 ‘로그 폴더’를 클릭하면 Windows 탐색기에서 진단 결과가 저장된 로그 폴더를 열 수 있습니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-10 162405.png" alt="" width="563"><figcaption></figcaption></figure>

&#x20;      진단 결과 전송이 완료되면 버튼이 ‘진단 결과 전송 완료’로 표시되며, 클릭할 수 없게 됩니다.

<figure><img src="../../.gitbook/assets/image (2251).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
&#x20;     **NOTE**\
&#x20;     · 전송에 실패한 경우, 30초 후에 한 번만 자동으로 재전송이 시도됩니다.\
&#x20;     · 환경 진단을 다시 실행하여 진단 결과를 전송하려면 ‘재진단 시작’을 클릭하십시오.\
&#x20;     · ‘DirectCloud 드라이브 환경 진단’ 화면을 닫으려면 오른쪽 상단의 ‘✕’를 클릭하십시오.
{% endhint %}



{% hint style="warning" %}
**DirectCloud 드라이브 환경 진단 결과**
{% endhint %}

<table><thead><tr><th width="282">항목</th><th>설명</th></tr></thead><tbody><tr><td>진단 일시</td><td>DirectCloud 드라이브 환경 진단을 실행한 날짜와 시간이 표시됩니다.</td></tr><tr><td>PC 환경</td><td>다음의 PC 환경 정보가 표시됩니다.<br>· 운영 체제<br>· 메모리<br>· CPU</td></tr><tr><td>프록시</td><td>프록시 사용 여부가 표시됩니다.<br>프록시를 사용하는 경우, 프록시의 IP 주소가 표시됩니다.</td></tr><tr><td>인터넷 속도</td><td>다음 항목에 대한 인터넷 속도가 측정되어 표시됩니다.<br>· 업로드<br>· 다운로드</td></tr><tr><td>외부 프로그램의 접근</td><td>최근 7일간 DirectCloud 드라이브의 파일에 접근한 외부 프로그램의 이름과 횟수가 표시됩니다.<br>접근이 많은 순서대로 최대 5개의 프로그램이 표시됩니다.</td></tr></tbody></table>
