---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-ai/enable_ai_folder
---

# 특정 폴더에서 DirectCloud AI를 활성화하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용해 Storage에서 필요한 정보를 빠르게 찾아내거나 정보를 요약하기 위한 옵션 서비스인 DirectCloud AI를 제공하고 있습니다.\
Web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하시면, 생성 AI가 대상이 되는 여러 파일을 참고하여 정보를 추출해 제공합니다.\
또한 DirectCloud AI에는 전자메일을 파일로 저장할 때 사용하는 파일 형식인 EML 파일을 EML 요약이 활성화된 폴더에 업로드하면, 내용을 질문과 답변 형식으로 요약해 텍스트 파일로 저장하는 기능이 있습니다. 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참고됩니다.\
이 매뉴얼에서는 관리자 페이지에서 특정 폴더에 DirectCloud AI를 활성화하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* DirectCloud AI에 공통되는 사양 및 주의 사항에 대해서는 [DirectCloud AI 사양 및 참고사항](https://help.directcloud.net/user_manual/specification/ai_specification)을 참조해 주시기 바랍니다.
* 관리자 권한이 부여된 사용자는 관리자 페이지의 'DirectCloud AI' 항목에 체크가 되어 있어야 합니다.
* 이 매뉴얼의 설정을 진행하시려면, [DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/admin_manual/directcloud-ai/enable_ai)에 따라 DirectCloud AI가 사용함으로 설정되어 있어야 합니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '공유설정'>  'Shared Box 관리' 메뉴를 클릭하고 DirectCloud AI를 활성화할 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2287).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 폴더 속성에서 DirectCloud AI 설정이 '사용 안함'으로 설정된 경우 수정 버튼을 클릭합니다. DirectCloud AI 설정이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2288).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. DirectCloud AI 설정에서 '사용'을 선택합니다.

{% hint style="info" %}
**NOTE**\
폴더에 확장자가 pdf, docx, txt인 파일이 있는 경우 생성 AI가 언어를 처리하는 데 사용하는 벡터 데이터가 자동으로 생성됩니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2289).png" alt=""><figcaption></figcaption></figure>



4. Guest에게 DirectCloud AI 사용을 허용하려면 '게스트 포함'에 체크합니다.

<figure><img src="../../.gitbook/assets/image (2290).png" alt=""><figcaption></figcaption></figure>



5. EML 파일을 요약하려는 경우에는 옵션의 'AI 요약'에 체크합니다.

{% hint style="info" %}
**NOTE**\
AI 요약에 체크하면 대상 폴더에 확장자 eml 파일을 업로드, 복사, 이동했을 때 내용이 질문과 답변 형식으로 요약되어 텍스트 파일로 저장됩니다. 이 요약 처리에도 토큰 또는 크레딧이 소모됩니다. 또한 요약된 텍스트 파일도 벡터 데이터 생성 대상이 됩니다.\
문서의 분량이나 파일 수에 따라 토큰 또는 크레딧이 소모되므로 주의해 주시기 바랍니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2291).png" alt=""><figcaption></figcaption></figure>



6. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2292).png" alt=""><figcaption></figcaption></figure>

폴더 속성의 DirectCloud AI 설정이 사용함으로 변경되며, DirectCloud AI를 이용할 수 있게 됩니다.\
또한 폴더 속성에서 버전 관리 표시가 사라집니다.

<figure><img src="../../.gitbook/assets/image (2293).png" alt=""><figcaption></figcaption></figure>
