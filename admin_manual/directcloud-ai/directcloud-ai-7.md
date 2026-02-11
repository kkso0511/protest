---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-ai/directcloud-ai-7
---

# DirectCloud AI의 챗봇 위젯 내역을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용하여 Storage에서 필요한 정보를 빠르게 검색하기 위한 옵션 서비스인 DirectCloud AI를 제공하고 있습니다.\
사용자 페이지에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하면, 생성 AI가 대상이 되는 여러 파일을 검색해 정보를 추출하여 제공합니다.\
또한 DirectCloud AI에는 전자메일을 파일로 저장할 때 사용되는 파일 형식인 EML 파일을 EML 요약이 활성화된 폴더에 업로드하면, 내용을 질문·답변 형식으로 요약해 텍스트 파일로 저장하는 기능이 있습니다. 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
DirectCloud AI가 활성화된 폴더에서는 목적과 용도에 따라 여러 개의 채팅룸을 생성할 수 있습니다. 또한 미리 예상되는 질문을 준비하고 특성 등을 설정하여 챗봇으로 활용할 수 있으며, 챗봇은 위젯 형태로 외부 Web 사이트에 설정할 수도 있습니다.\
DirectCloud의 폴더 및 챗봇 위젯에서 질문·답변 및 요약 기능을 사용할 때는 계약되어 있는 DirectCloud AI 플랜에 따라 토큰 또는 크레딧이 소모됩니다.\
이 매뉴얼에서는 관리 페이지의 'DirectCloud AI' > '챗봇 위젯 내역' 메뉴에서 생성한 챗봇 위젯의 내역을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '보안 정책'에 접근 할 수 있습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참조해 주시기 바랍니다.

***

### 절차

{% hint style="warning" %}
**챗봇 위젯 내역을 확인하기**
{% endhint %}

1. 'DirectCloud AI' > '챗봇 위젯 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2355).png" alt=""><figcaption></figcaption></figure>



2. 챗봇 위젯 내역을 확인합니다.

<table><thead><tr><th width="157.5">항목</th><th>설명</th></tr></thead><tbody><tr><td>챗봇명</td><td>위젯에서 사용되고 있는 챗봇의 이름이 표시됩니다.</td></tr><tr><td>폴더</td><td>위젯을 생성한 폴더의 경로가 표시됩니다.</td></tr><tr><td>사용자</td><td>위젯을 생성, 수정, 삭제한 사용자의 이름이 표시됩니다.<br>이름에 마우스 커서를 올리면 툴팁으로 사용자 ID를 확인할 수 있습니다.</td></tr><tr><td>일시</td><td>위젯을 생성, 수정, 삭제한 날짜와 시간이 표시됩니다.</td></tr><tr><td>이벤트</td><td>생성, 수정, 삭제 중 하나의 작업이 표시됩니다.</td></tr><tr><td>내역</td><td><p>위젯을 생성하거나 수정한 경우 상세 표시 버튼이 나타납니다.<br>상세 표시 버튼을 클릭하면 챗봇 위젯 내역 화면에서 다음과 같은 상세 작업 이력을 확인할 수 있습니다.<br></p><p>• 위젯 임베드 코드<br>• 작업(일시)<br>• 위젯 옵션<br>• 버튼 이미지 파일<br>• 세션당 최대 질문 수<br>• 종료일<br>• 비밀번호</p></td></tr></tbody></table>



{% hint style="warning" %}
**챗봇 위젯 내역을 필터링하여 표시하기**
{% endhint %}

챗봇 위젯 내역 화면에서는 챗봇 위젯의 생성 이력을 기간, 작업 종류, 챗봇 이름, 사용자 이름/사용자 ID, 폴더 이름, 표시 건수로 필터링하여 확인할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2356).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="102.79998779296875">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>챗봇 위젯 내역을 표시할 기간을 직전 7일, 직전 15일, 직전 1개월, 직전 3개월 중에서 선택합니다.</td></tr><tr><td>2</td><td>계약 시작일부터 현재까지의 챗봇 위젯 내역을 표시할 기간을 지정합니다.<br>지정할 수 있는 최대 기간은 12개월입니다.<br>단, 2024년 1월에 시작된 신규 요금제 기준으로 스탠다드 플랜 또는 어드밴스드 플랜을 계약한 경우, 이 설정은 표시되지 않습니다.</td></tr><tr><td>3</td><td>챗봇 위젯 내역을 작업 기준으로 필터링하려는 경우 생성, 수정, 삭제 중에서 선택합니다.</td></tr><tr><td>4</td><td>챗봇 위젯 내역을 필터링하려는 경우 챗봇 이름, 사용자 이름 또는 사용자 ID, 폴더 이름을 입력합니다.</td></tr><tr><td>5</td><td>챗봇 위젯 내역을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**챗봇 위젯 내역을 CSV 파일로 다운로드하기**
{% endhint %}

1. 챗봇 위젯 내역 설정에서 'CSV 다운로드' 버튼을 클릭합니다.\
   필터링하여 표시된 결과만 다운로드할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2357).png" alt=""><figcaption></figcaption></figure>



2. CSV 파일을 열어 정상적으로 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2358).png" alt=""><figcaption></figcaption></figure>
