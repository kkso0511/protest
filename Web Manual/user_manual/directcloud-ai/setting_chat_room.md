---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/directcloud-ai/setting_chat_room
---

# DirectCloud AI의 채팅룸을 설정하는 방법

### 개요

DirectCloud에서는 생성 AI를 활용하여 Storage 내에서 필요한 정보를 빠르게 검색하거나 요약할 수 있는 옵션 서비스인 DirectCloud AI를 제공합니다.\
web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하면, 생성 AI가 해당 폴더 내 여러 파일을 참조하여 관련 정보를 추출하고 제시합니다.\
또한 DirectCloud AI에는 이메일을 파일로 저장할 때 사용하는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 내용을 질문과 답변 형식으로 요약하여 텍스트 파일로 저장하는 기능이 있습니다.\
이렇게 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
DirectCloud AI가 활성화된 폴더에서는 목적이나 용도에 따라 여러 개의 채팅룸을 생성할 수 있습니다. 또한 미리 예상되는 질문을 설정해 두면 챗봇으로도 활용할 수 있습니다.\
이 매뉴얼에서는 사용자 페이지에서 DirectCloud AI가 활성화된 폴더 내에서 채팅룸을 생성하고 편집하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼의 절차를 따라 DirectCloud AI를 사용하려면 다음 설정이 완료되어 있어야 합니다.
  * 관리자 페이지의 'DirectCloud AI'->'설정' 에서 DirectCloud AI 를 '사용' 으로 설정
  * 폴더 속성의 ‘DirectCloud AI’를 ‘사용함’으로 설정
  * [DirectCloud AI를 사용하기 위한 파일을 준비하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/file_preparation) 절차에 따라 DirectCloud AI의 처리 대상 파일 준비 완료
* Web 애플리케이션에서 DirectCloud AI를 사용하는 방법은 다음 두 가지입니다.
  1. [사용자 페이지의 특정 폴더에서 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/activation)에 따라 DirectCloud AI가 활성화된 폴더의 슬라이드 화면에서 ‘DirectCloud AI’ 탭을 표시하는 방법
  2. DirectCloud AI Home을 표시하는 방법
* 채팅을 통해 질문하는 사용자는 DirectCloud AI가 ‘사용함’으로 설정된 폴더에 대해 <마스터>, <전체권한>, <편집자>, <편집자－>, <다운로더>, <프리뷰어＋>, <프리뷰어> 접근 권한이 부여되어 있어야 합니다.
* 사용 중인 GPT 모델의 사양이나 질문 방식, 질문 시점 등에 따라 DirectCloud AI로부터 기대한 정보를 얻지 못하거나 부자연스러운 답변이 반환될 수 있습니다.\
  이 경우, ‘상세하게’, ‘간략하게’ 등 질문 방식을 바꿔 여러 번 시도해 보는 것을 권장합니다.
* 챗봇을 설정하는 사용자는 <마스터> 권한이 부여되어 있어야 합니다.

***

### 절차

{% hint style="warning" %}
**채팅룸의 기본 구성**
{% endhint %}

* Shared Box의 슬라이드 화면에 있는 DirectCloud AI 탭

<figure><img src="../../.gitbook/assets/image (2234).png" alt=""><figcaption></figcaption></figure>



* DirectCloud AI Home

<figure><img src="../../.gitbook/assets/image (2235).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="90.5999755859375">No.</th><th width="161.60003662109375">설정 항목</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>채팅룸 표시 영역</td><td>채팅룸을 표시하거나 설정을 진행하는 영역입니다.</td></tr><tr><td>❷</td><td>채팅룸 이름</td><td><p>이름을 클릭하면 목록에서 기존 채팅룸으로 전환할 수 있습니다.<br>작업 시점에 따라 아래와 같은 이름이 표시될 수 있습니다.<br></p><p>&#x3C;새 대화><br>채팅 기록이 없는 경우에 표시됩니다. 또한 기존 채팅룸이 있을 때 신규 채팅룸을 클릭하여 새 채팅룸을 생성할 수 있습니다.<br></p><p>&#x3C;Saved chat><br>2025년 8월 20일 업데이트 이전에 채팅을 사용한 이력이 있는 경우, 해당 채팅룸이 자동으로 이 이름으로 저장됩니다.<br></p><p>&#x3C;자동으로 설정된 채팅룸 이름><br>채팅 대화 내용에 따라 DirectCloud AI가 자동으로 생성한 이름이 표시됩니다.</p></td></tr><tr><td>❸</td><td>설정 버튼</td><td>설정 버튼을 클릭하면 채팅룸 설정과 관련된 채팅룸 이름 변경, 채팅룸 삭제, 챗봇 설정 항목을 선택할 수 있습니다.<br><br><strong>NOTE</strong><br>Shared Box의 슬라이드 화면에 있는 DirectCloud AI 탭에만, 설정 버튼 왼쪽에 ‘DirectCloud AI Home에서 표시’ 버튼이 있습니다.<br>이 버튼을 클릭하면 별도의 DirectCloud AI Home 탭에서 해당 폴더를 표시할 수 있습니다.<br></td></tr><tr><td>❹</td><td>챗봇 설정 내용</td><td>채팅 기록이 없는 경우, ❸의 ‘챗봇 설정’에서 설정한 내용이 표시됩니다.</td></tr><tr><td>❺</td><td>채팅 입력란</td><td>DirectCloud AI에 대한 질문을 입력합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**새 채팅룸 만들기**
{% endhint %}

아래 단계에서는 DirectCloud AI Home 화면을 기준으로 설명하지만, Shared Box의 슬라이드 화면에 있는 DirectCloud AI 탭에서도 동일한 절차로 조작할 수 있습니다.

1. 채팅룸 이름을 클릭하고 ‘＋새 대화’을 선택합니다.

{% hint style="info" %}
**NOTE**\
채팅룸 이름에 ‘새 대화’가 표시되어 있는 경우에는 ‘＋새 대화’ 선택할 수 없습니다.\
최대 10개의 채팅룸을 생성할 수 있습니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2236).png" alt=""><figcaption></figcaption></figure>



2. 새 대화가 나타납니다.

<figure><img src="../../.gitbook/assets/image (2237).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**채팅룸 설정**
{% endhint %}

**\[채팅룸 이름 바꾸기]**

1. 이름을 변경하려는 채팅룸을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2238).png" alt=""><figcaption></figcaption></figure>



2. 설정 버튼을 클릭하고 ‘대화명 수정’을 선택합니다.

{% hint style="info" %}
**NOTE:** ‘새 대화’이 표시되어 있고 아직 한 번도 대화가 없는 경우에는 ‘대화명 수정’을 선택할 수 없습니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2239).png" alt=""><figcaption></figcaption></figure>



3. 채팅룸 이름을 20자 이내로 입력한 후 ‘이름 변경’ 버튼을 클릭합니다.\
   채팅룸의 이름이 변경됩니다.

<figure><img src="../../.gitbook/assets/image (2240).png" alt=""><figcaption></figcaption></figure>



**\[채팅룸 삭제]**

1. 삭제하려는 채팅룸을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2238).png" alt=""><figcaption></figcaption></figure>



2. 설정 버튼을 클릭하고 ‘대화 삭제’를 선택합니다.

{% hint style="info" %}
**NOTE:** ‘새 대화’가 표시되어 있고 아직 한 번도 대화가 없는 경우에는 ‘대화 삭제’를 선택할 수 없습니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2243).png" alt=""><figcaption></figcaption></figure>



3. 삭제 확인 화면에서 ‘삭제’ 버튼을 클릭합니다.\
   채팅룸이 삭제되고 ‘새 대화’가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2242).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**챗봇설정**
{% endhint %}

DirectCloud AI에서는 DirectCloud AI가 활성화된 폴더마다 하나의 챗봇을 설정할 수 있습니다.\
‘처음 표시되는 질문’과 ‘챗봇 설명’은 해당 폴더에 접근할 수 있는 사용자가 새로 생성된 채팅룸에 처음 접근했을 때 표시됩니다.

1. 설정 버튼을 클릭하고 ‘챗봇 설정’을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2244).png" alt=""><figcaption></figcaption></figure>



2. 챗봇 설정을 완료한 후 ‘저장’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2245).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2246).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="215.5999755859375">항목</th><th>설명</th></tr></thead><tbody><tr><td>챗봇 이미지 <img src="https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000C7Tx&#x26;feoid=00N2w00000JMb2T&#x26;refid=0EMQ800000IFKAY" alt="" data-size="line"></td><td>클릭하면 PC 내의 이미지 파일을 선택하여 챗봇 이미지를 설정할 수 있습니다. 10MB 이하의 JPEG, PNG, GIF 형식의 이미지 파일을 업로드할 수 있습니다. 세로와 가로 비율이 1:1(정사각형)인 이미지를 설정하는 것을 권장합니다.</td></tr><tr><td>챗봇 이름</td><td>챗봇 이름을 50자 이내로 입력합니다. 기본적으로 Shared Box의 이름이 설정되어 있습니다.</td></tr><tr><td>챗봇 설명</td><td>챗봇 설명을 100자 이내로 입력합니다.</td></tr><tr><td>대화 스타터</td><td>DirectCloud AI의 챗봇에서는 예상되는 질문을 최대 10개까지 설정할 수 있습니다. 입력란에 문자를 입력하면 다음 입력란이 표시됩니다. 각 입력란에는 500자 이내의 질문을 입력할 수 있습니다. 입력란 오른쪽 상단의 ‘✕’ 버튼을 클릭하면, 입력란을 삭제할 수 있습니다.</td></tr><tr><td>챗봇 역할</td><td>챗봇의 대화 방식을 변경합니다.<br><br>기본<br>CS지원: 공손하고 차분하며, 공감하는 태도<br>영업 보조: 자신감있고, 설득력 있는말투,  친근하면서도 전문적<br>마케팅 보조: 창의적이고 활기찬 말투, 트렌디하고 긍정적<br>관리 부서: 신뢰감 있고 전문적인 말투, 간결하고 명확</td></tr><tr><td>답변길이</td><td>챗봇의 답변의 길이를 정합니다.</td></tr></tbody></table>

챗봇 설정이 완료되었습니다.
