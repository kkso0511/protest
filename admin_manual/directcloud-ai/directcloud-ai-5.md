---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-ai/directcloud-ai-5
---

# DirectCloud AI의 답변 평가 이력을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용하여 Storage에서 필요한 정보를 빠르게 검색하기 위한 옵션 서비스인 DirectCloud AI를 제공하고 있습니다.\
사용자 페이지에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하면, 생성 AI가 대상이 되는 여러 파일을 검색하여 정보를 추출해 제공하는 방식입니다.\
또한 DirectCloud AI에는 전자메일을 파일로 저장할 때 사용되는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 그 내용을 질문과 답변 형식으로 요약하여 텍스트 파일로 저장하는 기능이 있습니다. 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
DirectCloud AI가 활성화된 폴더에서는 목적이나 용도에 따라 여러 개의 채팅룸을 생성할 수 있습니다. 또한 미리 예상되는 질문을 준비하고 특성 등을 설정하여 챗봇으로 활용할 수도 있습니다. 챗봇은 위젯으로 외부 Web사이트에 설정할 수도 있습니다.\
DirectCloud의 폴더 및 챗봇 위젯에서 질문·답변 또는 요약을 수행할 때는 계약되어 있는 DirectCloud AI 플랜에 따라 토큰 또는 크레딧이 소모됩니다.\
이 매뉴얼에서는, 답변 평가가 활성화되어 있는 환경에서 관리 페이지의 'DirectCloud AI' > 'AI 답변 평가 내역' 메뉴에서 답변 평가 이력을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '보안 정책'에 접근 할 수 있습니다.
* 관리 페이지의 'DirectCloud AI' > '설정' 메뉴에서 답변 평가가 사용하지 않음으로 설정되어 있는 경우에는 답변 평가 이력 메뉴가 표시되지 않습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참조해 주시기 바랍니다.

***

### 절차

{% hint style="warning" %}
**DirectCloud AI의 답변 평가 이력을 확인하기**
{% endhint %}

**\[답변 평가 이력 화면을 표시하기]**

1. 'DirectCloud AI' > 'AI 답변 평가 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (288).png" alt=""><figcaption></figcaption></figure>



**\[폴더에서 AI 답변 평가 내역을 확인하기]**

1. '폴더 질의응답'탭을 선택한 후 AI 답변 평가 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (285).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="161">항목</th><th>내용</th></tr></thead><tbody><tr><td>사용자</td><td>AI 답변 평가를 수행한 사용자가 사용자 ID(메일 주소) 형식으로 표시됩니다.</td></tr><tr><td>평가 일시</td><td>사용자가 AI 답변 평가를 수행한 일시가 표시됩니다.</td></tr><tr><td>GPT Model</td><td>평가 대상이 된 대화에서 사용된 GPT 모델이 표시됩니다.<br>GPT 모델의 종류는 아래와 같습니다.<br>· GPT-4 / 8K<br>· GPT-4 / 32K<br>· GPT-4o<br>· GPT-4o-mini<br>· GPT-o3-mini<br>· GPT-4.1<br>· GPT-4.1-mini<br>· GPT-5<br>· GPT-5-mini</td></tr><tr><td>질문</td><td><p>사용자가 평가한 질문이 표시됩니다.<br>질문 문자열이 길 경우, 마우스 커서를 올리면 툴팁으로 내용을 확인할 수 있습니다.</p><p>링크를 클릭하면 답변 상세 화면에서 아래 정보를 확인할 수 있습니다.<br>· 사용자<br>· 평가<br>· Bad 평가의 이유<br>· 질문<br>· 답변</p><p><br>NOTE:<br>위의 정보 외에도 참조된 파일과 데이터 청크를 확인할 수 있습니다.</p></td></tr><tr><td>평가</td><td>다음 중 하나의 평가가 표시됩니다.<br>· Good<br>· Bad</td></tr></tbody></table>



**\[위젯에서 사용 이력을 확인하기]**

1. '챗봇위젯' 탭을 선택한 후 AI 답변 평가 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (287).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="161">항목</th><th>내용</th></tr></thead><tbody><tr><td>사용자</td><td>AI 답변 평가를 수행한 사용자가 사용자 ID(메일 주소) 형식으로 표시됩니다.</td></tr><tr><td>진입 경로</td><td>챗봇 위젯을 설치한 Web페이지의 URL이 표시됩니다.</td></tr><tr><td>평가 일시</td><td>사용자가 AI 답변 평가를 수행한 일시가 표시됩니다.</td></tr><tr><td>GPT Model</td><td>평가 대상이 된 대화에서 사용된 GPT 모델이 표시됩니다.<br>GPT 모델의 종류는 아래와 같습니다.<br>· GPT-4 / 8K<br>· GPT-4 / 32K<br>· GPT-4o<br>· GPT-4o-mini<br>· GPT-o3-mini<br>· GPT-4.1<br>· GPT-4.1-mini<br>· GPT-5<br>· GPT-5-mini</td></tr><tr><td>질문</td><td><p>사용자가 평가한 질문이 표시됩니다.<br>질문 문자열이 길 경우, 마우스 커서를 올리면 툴팁으로 내용을 확인할 수 있습니다.</p><p>링크를 클릭하면 답변 상세 화면에서 아래 정보를 확인할 수 있습니다.<br>· 사용자<br>· 평가<br>· Bad 평가의 이유<br>· 질문<br>· 답변</p><p><br>NOTE:<br>위의 정보 외에도 참조된 파일과 데이터 청크를 확인할 수 있습니다.</p></td></tr><tr><td>평가</td><td>다음 중 하나의 평가가 표시됩니다.<br>· Good<br>· Bad</td></tr></tbody></table>



{% hint style="warning" %}
**DirectCloud AI의 AI 답변 평가 내역을 필터링하여 표시하기**
{% endhint %}

DirectCloud AI 사용 이력 화면에서는 폴더 탭 또는 위젯 탭을 선택하여 각각의 사용 이력을 필터링해 표시할 수 있습니다.\
이 매뉴얼에서는 폴더 탭 화면을 예로 설명하고 있지만, 위젯 탭 화면에서도 동일하게 설정할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (283).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="89.5">No.</th><th>내용</th></tr></thead><tbody><tr><td>1</td><td>클릭하여 드롭다운 리스트를 표시하고, 아래 평가 중 하나를 선택합니다.<br>기본값은 전체가 선택되어 있어 모든 평가가 검색 대상이 됩니다.<br>· 좋은 응답<br>· 별로인 응답</td></tr><tr><td>2</td><td>클릭하여 드롭다운 리스트를 표시하고, Bad 평가의 이유를 선택합니다.<br>기본값은 전체가 선택되어 있어 모든 Bad 평가 이유가 검색 대상이 됩니다.</td></tr><tr><td>3</td><td>클릭하여 드롭다운 리스트를 표시하고, 아래 GPT 모델 중 하나를 선택합니다.<br>기본값은 모든 GPT 모델이 선택되어 있어, 모든 모델이 검색 대상이 됩니다.<br>· GPT-4 / 8K<br>· GPT-4 / 32K<br>· GPT-4o<br>· GPT-4o-mini<br>· GPT-o3-mini<br>· GPT-4.1<br>· GPT-4.1-mini<br>· GPT-5<br>· GPT-5-mini</td></tr><tr><td>4</td><td><p>선택한 탭에 따라 DirectCloud AI의 AI 답변 평가 내역을 필터링할 수 있습니다.</p><p>· '폴더 질의응답'탭: 평가를 수행한 사용자의 이름 또는 사용자 ID</p><p>· '챗봇 위젯' 탭: 사용자(챗봇 위젯을 이용한 사용자에게 자동 부여되는 고유 값), 설치 위치</p></td></tr><tr><td>5</td><td>DirectCloud AI의 AI 답변 평가 내역 표시 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**AI 답변 평가 내역을 CSV 파일로 다운로드 하기**
{% endhint %}

이 매뉴얼에서는 '폴더 질의응답'탭을 예로 들어 다운로드 절차를 설명하고 있지만, '챗봇 위젯'탭에서도 동일한 방식으로 작업할 수 있습니다.

1. 'AI 답변 평가 내역' 에서 'CSV 다운로드' 버튼을 클릭합니다.\
   필터링하여 표시된 결과만 다운로드할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (284).png" alt=""><figcaption></figcaption></figure>



2. CSV 파일을 열어 정상적으로 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2348).png" alt=""><figcaption></figcaption></figure>
