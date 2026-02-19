---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-ai/enable_ai
---

# DirectCloud AI를 활성화하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용해 Storage에서 필요한 정보를 빠르게 찾아내거나, 정보를 요약하기 위한 옵션 서비스인 DirectCloud AI를 제공하고 있습니다.\
Web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하시면, 생성 AI가 대상이 되는 여러 파일을 참고하여 필요한 정보를 추출해 제공합니다.\
또한 DirectCloud AI에는 전자메일을 파일로 저장할 때 사용하는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 내용을 질문과 답변 형식으로 요약하여 텍스트 파일로 저장하는 기능이 있습니다. 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참고됩니다.\
이 매뉴얼에서는 관리자 페이지에서 DirectCloud AI를 활성화하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* DirectCloud AI에 공통되는 사양 및 주의 사항에 대해서는 [DirectCloud AI 사양 및 참고사항](https://help.directcloud.net/user_manual/specification/ai_specification)을 참조해 주시기 바랍니다.
* 관리자 권한이 부여된 사용자는 관리자 페이지의 'DirectCloud AI' 항목에 체크가 되어 있어야 합니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**DirectCloud AI 사용 설정**
{% endhint %}

1. 'DirectCloud AI' > '설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (346).png" alt=""><figcaption></figcaption></figure>



2. DirectCloud AI 설정에서 '사용'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (347).png" alt=""><figcaption></figcaption></figure>



3. GPT Model 드롭다운 목록에서 DirectCloud AI의 채팅에서 GPT가 답변을 생성할 때 사용할 GPT 모델을 선택합니다. 아래 중 하나의 버전을 선택할 수 있습니다.

* GPT-4o
* GPT-4o-mini
* GPT-o3-mini
* GPT-4.1
* GPT-4.1-mini
* GPT-5(Beta)
* GPT-5-mini(Beta)

<figure><img src="../../.gitbook/assets/image (348).png" alt=""><figcaption></figcaption></figure>



4. DirectCloud AI의 채팅에서 질문할 때, 이전 질문과 답변의 텍스트를 참조할 수 있도록 하려는 경우에는, '질문시 이전 대화 참고'에 체크합니다.

<figure><img src="../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>



5. 챗봇위젯을 사용하는 경우에는, '사용'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>



6. DirectCloud AI의 답변을 평가하는 경우에는, '답변 평가'의 '사용'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**NOTE**\
답변 평가 기능에서 '사용'을 선택한 뒤 저장 버튼을 클릭하면 정보 수집에 관한 동의 화면이 표시됩니다. '동의' 버튼을 클릭하여 질문, 답변, 참고에 관한 데이터를 수집하는 것에 동의하시면 답변 평가 기능을 이용할 수 있게 됩니다.\
답변 평가 기능을 사용할 수 있게 되면 Web 브라우저의 DirectCloud AI 채팅에서 질문을 했을 때, 답변에 평가 버튼이 표시됩니다.
{% endhint %}



7. 원본 파일 수정 없이 AI 데이터를 관리 하려면 'AI 데이터 관리'를 '사용' 으로 선택합니다.

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>



8. '저장' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>



9. 관리 페이지 및 사용자 페이지의 폴더 속성에 'DirectCloud AI'가 표시되어 있는지 확인합니다.\
   자세한 내용은 [특정 폴더에서 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/admin_manual/directcloud-ai/enable_ai_folder) 및 [사용자 페이지의 특정 폴더에서 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/activation)을 참조해 주십시오.
