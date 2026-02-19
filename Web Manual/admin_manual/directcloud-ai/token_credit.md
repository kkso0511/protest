---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-ai/token_credit
---

# DirectCloud AI에서 사용한 토큰/크레딧을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용해 Storage에서 필요한 정보를 빠르게 찾아낼 수 있는 옵션 서비스인 DirectCloud AI를 제공하고 있습니다.\
사용자 페이지에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하시면, 생성 AI가 대상이 되는 여러 파일을 검색하여 정보를 추출해 제공합니다.\
또한 DirectCloud AI에는 전자메일을 파일로 저장할 때 사용되는 파일 형식인 EML 파일을 EML 요약이 활성화된 폴더에 업로드하면, 내용을 질문과 답변 형식으로 요약해 텍스트 파일로 저장하는 기능이 있습니다. 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참고됩니다.\
DirectCloud AI가 활성화된 폴더에서는 목적이나 용도에 따라 여러 개의 채팅룸을 생성할 수 있습니다. 또한 미리 예상되는 질문을 준비해 두면 챗봇처럼 활용할 수도 있습니다.\
채팅룸에서의 질문·답변과 요약 기능은 계약 중인 DirectCloud AI의 플랜에 따라 토큰 또는 크레딧이 소모됩니다.\
이 매뉴얼에서는 관리자 페이지의 'DirectCloud AI' > 'AI 사용량' 이력에서 소모된 토큰 또는 크레딧의 이력을 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* DirectCloud AI에 공통되는 사양 및 주의 사항에 대해서는 [DirectCloud AI 사양 및 참고사항](https://help.directcloud.net/user_manual/specification/ai_specification)을 참조해 주시기 바랍니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**DirectCloud AI 사용 기록 보기**
{% endhint %}

1. 'DirectCloud AI' > 'AI 사용량' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2294).png" alt=""><figcaption></figcaption></figure>



2. DirectCloud AI의 사용 이력을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2295).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="203.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>구분</td><td><p>다음 중 하나의 구분이 표시됩니다.</p><ul><li>질의응답</li><li>요약</li></ul></td></tr><tr><td>파일/폴더</td><td>구분이 '질의응답'인 경우 DirectCloud AI 대상 폴더의 경로가 표시됩니다.<br>구분이 '요약'인 경우 요약 후 생성된 텍스트 파일과 DirectCloud AI 대상 폴더의 경로가 표시됩니다.</td></tr><tr><td>사용자</td><td>채팅룸을 생성한 사용자의 이름이 표시됩니다.<br>사용자 이름에 마우스 커서를 올리면 툴팁으로 사용자 ID를 확인할 수 있습니다.</td></tr><tr><td>완료 일시</td><td>DirectCloud AI의 채팅룸에서 해당 구분의 처리가 완료된 날짜와 시간이 표시됩니다.</td></tr><tr><td>GPT Model</td><td>해당 구분의 처리에 사용된 GPT 모델이 표시됩니다.</td></tr><tr><td>결과</td><td><p>다음 중 하나의 결과가 표시됩니다.</p><ul><li>성공</li><li>실패</li></ul></td></tr><tr><td>입력 토큰</td><td>채팅룸에서 질문에 사용된 토큰 수가 표시됩니다.</td></tr><tr><td>출력 토큰</td><td>채팅룸에서의 답변 및 요약에 사용된 토큰 수가 표시됩니다.</td></tr><tr><td>사용 크레딧</td><td>채팅룸의 질문·답변 및 요약에서 사용된 크레딧 수가 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**DirectCloud AI의 사용 이력을 조건에 따라 필터링하여 표시하기**
{% endhint %}

DirectCloud AI의 사용 이력 화면에서는 DirectCloud AI의 사용 이력을 기간, 구분, GPT 모델, 채팅룸 생성자, 파일·폴더 이름, 폴더 경로, 건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2296).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="114">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>DirectCloud AI의 사용 이력을 표시할 기간을 최근 7일, 최근 15일, 최근 1개월, 최근 3개월 중에서 선택합니다.</td></tr><tr><td>2</td><td>계약 시작일부터 현재까지의 DirectCloud AI 사용 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 최대 12개월입니다.</td></tr><tr><td>3</td><td><p>클릭하여 드롭다운 목록을 표시한 뒤, 아래 구분 중 하나를 선택합니다.<br>기본적으로는 모든 구분이 선택되어 있어 전체가 검색 대상이 됩니다.</p><ul><li>질의응답</li><li>요약</li></ul></td></tr><tr><td>4</td><td>클릭하여 드롭다운 목록을 표시하고 GPT 모델 중 하나를 선택합니다.<br>기본적으로는 모든 GPT 모델이 선택되어 있어 전체가 검색 대상이 됩니다.</td></tr><tr><td>5</td><td>DirectCloud AI의 사용 이력을 채팅룸 생성자 또는 파일·폴더 이름으로 필터링하려는 경우, 사용자 이름 또는 사용자 ID, 파일 이름, 폴더 이름, 또는 폴더 경로를 입력합니다.</td></tr><tr><td>6</td><td>DirectCloud AI의 사용 이력을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**DirectCloud AI의 사용 이력을 CSV 파일로 다운로드 하기**
{% endhint %}

1. 'AI 사용량'에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드 됩니다.\
   DirectCloud AI의 사용 이력은 데이터가 방대해질 수 있으므로, 먼저 조건을 지정해 필터링한 뒤 다운로드를 진행하시는 것을 권장합니다.

<figure><img src="../../.gitbook/assets/image (2297).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. CSV 파일을 열어 내용이 문제 없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2298).png" alt=""><figcaption></figcaption></figure>
