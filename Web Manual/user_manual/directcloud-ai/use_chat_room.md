---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/directcloud-ai/use_chat_room
---

# DirectCloud AI의 채팅룸을 이용하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성형 AI를 활용하여 스토리지에서 필요한 정보를 빠르게 찾아내거나 요약할 수 있는 옵션 서비스인 DirectCloud AI를 제공합니다.\
Web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 궁금한 점을 입력하면, 생성형 AI가 해당 폴더 내 여러 파일을 참조하여 관련 정보를 추출하고 제시합니다.\
또한 DirectCloud AI에는 이메일을 파일로 저장할 때 사용되는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 그 내용을 질문과 답변 형식으로 요약해 텍스트 파일로 저장하는 기능이 있습니다. 이 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
이 매뉴얼에서는 Web 브라우저의 DirectCloud AI가 활성화된 폴더의 채팅을 통해 DirectCloud AI에 질문하고, 답변을 받는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼의 절차를 따라 DirectCloud AI를 사용하려면 다음 설정이 완료되어 있어야 합니다.
  * 관리자 페이지의 'DirectCloud AI'->'설정' 에서 DirectCloud AI 를 '사용' 으로 설정
  * 폴더 속성의 ‘DirectCloud AI’를 ‘사용함’으로 설정
  * [DirectCloud AI를 사용하기 위한 파일을 준비하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/file_preparation) 절차에 따라 DirectCloud AI의 처리 대상 파일 준비 완료
* Web 브라우저에서 DirectCloud AI를 사용하는 방법은 다음 두 가지입니다.
  1. [사용자 페이지의 특정 폴더에서 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/activation)에 따라 DirectCloud AI가 활성화된 폴더의 슬라이드 화면에서 ‘DirectCloud AI’ 탭을 표시하는 방법
  2. DirectCloud AI Home을 표시하는 방법
* 채팅을 통해 질문하는 사용자는 DirectCloud AI가 ‘사용함’으로 설정된 폴더에 대해 <마스터>, <전체권한>, <편집자>, <편집자－>, <다운로더>, <프리뷰어＋>, <프리뷰어> 접근 권한이 부여되어 있어야 합니다.
* 사용 중인 GPT 모델의 사양이나 질문 방식, 질문 시점 등에 따라 DirectCloud AI로부터 기대한 정보를 얻지 못하거나 부자연스러운 답변이 반환될 수 있습니다.\
  이 경우, ‘상세하게’, ‘간략하게’ 등 질문 방식을 바꿔 여러 번 시도해 보는 것을 권장합니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="info" %}
**DirectCloud AI의 채팅룸을 표시하기**
{% endhint %}

**\[DirectCloud AI가 활성화된 폴더에서 표시하기]**

1. Shared Box 메뉴를 클릭하고, 채팅을 시작하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2227).png" alt=""><figcaption></figcaption></figure>



2. 슬라이드 화면에서 ‘DirectCloud AI’ 탭을 클릭합니다.\
   DirectCloud AI의 채팅이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2228).png" alt=""><figcaption></figcaption></figure>



**\[DirectCloud AI Home에서 표시하기]**

1. DirectCloud AI Home을 표시하고, ‘DirectCloud AI 폴더’ 영역에서 채팅을 시작하려는 폴더를 클릭합니다.\
   ‘채팅룸’ 영역에 DirectCloud AI의 채팅이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2229).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**채팅룸에서 DirectCloud AI에 질문하기**
{% endhint %}

채팅룸에 DirectCloud AI에 대한 질문을 입력하면, 벡터 데이터가 생성된 모든 파일을 기반으로 DirectCloud AI가 답변을 제공합니다.

1. 목적에 맞는 채팅룸을 선택합니다.\
   새로운 채팅룸을 생성할 수도 있습니다. 자세한 내용은 ‘DirectCloud AI의 채팅룸을 설정하는 방법’을 참조하십시오.



2. 텍스트 상자에 질문을 입력한 뒤 Enter 키를 누르거나 ‘보내기’ 버튼을 클릭합니다.\
   질문 내용이나 대상 파일 등에 따라 답변이 반환되기까지 시간이 걸릴 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2230).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**NOTE**\
챗봇에 ‘처음 표시되는 질문’이 설정되어 있는 경우, 제시된 질문을 클릭할 수 있습니다.
{% endhint %}



3. DirectCloud AI의 답변을 확인하세요.

<figure><img src="../../.gitbook/assets/image (2232).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="75">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>‘챗봇 이름’이 표시됩니다. ‘챗봇 이름’이 설정되어 있지 않은 경우에는 ‘DirectCloud AI’로 표시됩니다.</td></tr><tr><td>❷</td><td>DirectCloud AI의 답변 일시가 표시됩니다.</td></tr><tr><td>❸</td><td>DirectCloud AI의 답변이 표시됩니다.<br>답변의 끝에는 참조한 파일 이름과 페이지 번호가 표시됩니다.<br>파일 이름을 클릭하면 미리보기 화면에서 내용을 확인할 수 있습니다.<br>파일 이름이 중간에서 잘려 보이는 경우, 파일 이름 위에 커서를 올리면 툴팁으로 전체 파일 이름을 확인할 수 있습니다.<br>참조된 파일이 많은 경우, ‘열기’ 또는 ‘닫기’ 버튼을 클릭하여 파일 목록을 표시하거나 숨길 수 있습니다.</td></tr></tbody></table>



{% hint style="warning" %}
&#x20;**DirectCloud AI 답변 평가**
{% endhint %}

이 매뉴얼에서는 ‘답변 평가’가 활성화되어 있는 경우, DirectCloud AI의 답변을 평가하는 절차에 대해 설명합니다.\
답변을 평가하려면 슬라이드 화면의 ‘DirectCloud AI’ 탭에서 평가하려는 답변을 표시합니다.

**\[Good 평가]**

Good 평가를 하려면  <img src="https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000CH6j&#x26;feoid=00N2w00000JMb2T&#x26;refid=0EMQ800000DCdFp" alt="" data-size="line"> 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (404).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**NOTE**\
입력된 평가는 변경할 수 없습니다.
{% endhint %}



**\[Bad 평가]**

1. Bad 평가를 하려면 <img src="https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000CH6j&#x26;feoid=00N2w00000JMb2T&#x26;refid=0EMQ800000DCfEP" alt="" data-size="line"> 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (405).png" alt=""><figcaption></figcaption></figure>

Bad 평가 이유의 선택지가 표시됩니다.\
상황에 따라 다음 절차로 진행합니다.

➡️ 해당하는 이유가 있는 경우: 2단계로 이동\
➡️ 해당하는 이유가 없는 경우: 3단계로 이동\
➡️ 해당 사유에 대해 자세한 정보를 입력하려는 경우: 4단계로 이동



2. 해당하는 Bad 평가 사유를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (406).png" alt=""><figcaption></figcaption></figure>



3. 해당하는 이유가 없는 경우에는 다음 절차로 평가를 진행합니다.

❶ ‘더 자세히..’ 를 클릭합니다. 자세한 이유를 설정하는 대화 상자가 표시됩니다.&#x20;

<figure><img src="../../.gitbook/assets/image (407).png" alt=""><figcaption></figcaption></figure>



❷ ‘기타’를 선택하고, 필요에 따라 텍스트 상자에 Bad 평가 사유를 입력한 뒤 ‘제’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (409).png" alt=""><figcaption></figcaption></figure>



4. 선택한 사유에 대해 자세한 정보를 입력하려는 경우에는 다음 절차로 평가를 진행합니다.

❶ ‘더 자세히...’를 클릭합니다. 자세한 이유를 설정하는 대화 상자가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (407).png" alt=""><figcaption></figcaption></figure>

❷ Bad 평가 사유를 선택하고, 텍스트 상자에 Bad 평가의 구체적인 이유를 입력한 뒤 ‘보내기’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (410).png" alt=""><figcaption></figcaption></figure>

\
**\[질문과 답변의 텍스트를 복사하기]**

복사하려는 질문 또는 답변에 마우스 커서를 올리고, 오른쪽 상단에 표시된 ‘복사’ 버튼을 클릭합니다.\
텍스트의 일부를 선택한 뒤 Ctrl+C 키를 눌러 복사할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (2233).png" alt=""><figcaption></figcaption></figure>

텍스트가 클립보드에 복사됩니다.\
복사한 텍스트는 메모장 등 다른 애플리케이션에 붙여넣을 수 있습니다.
