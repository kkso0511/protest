---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/directcloud-ai/activation
---

# 사용자 페이지의 특정 폴더에서 DirectCloud AI를 활성화하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용하여 Storage 내에서 필요한 정보를 빠르게 검색하거나 요약할 수 있는 옵션 서비스인 DirectCloud AI를 제공합니다.\
Web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하면, 생성 AI가 해당 폴더의 여러 파일을 참조하여 관련 정보를 추출하고 제시합니다.\
또한 DirectCloud AI에는 이메일을 파일로 저장할 때 사용하는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 내용을 질문과 답변 형식으로 요약하여 텍스트 파일로 저장하는 기능이 있습니다.\
이렇게 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
이 매뉴얼에서는 사용자 페이지의 지정된 폴더에서 DirectCloud AI를 활성화하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 사용자 페이지의 폴더 속성에서 DirectCloud AI 설정을 수행하는 사용자에게는 <마스터> 권한이 설정되어 있어야 합니다.
* ‘DirectCloud AI’ 설정은 기본적으로 ‘사용하지 않음’으로 설정되어 있습니다.
* 이 매뉴얼의 설정을 진행 하려면 먼저관리 페이지의 ‘DirectCloud AI’ > ‘설정’ 메뉴에서 ‘사용’을 선택해야 합니다.
* ‘DirectCloud AI'가 ‘사용함’으로 설정된 폴더가 있는 경우, 관리 페이지의 ‘DirectCloud AI’ > ‘설정’ 메뉴에서 ‘사용 안함’을 선택할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. Shared Box 메뉴를 클릭하고, DirectCloud AI를 설정하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (412).png" alt=""><figcaption></figcaption></figure>



2. 슬라이드 화면에서 DirectCloud AI의 설정 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (413).png" alt=""><figcaption></figcaption></figure>



3. '사용함'을 선택하고 확인 버튼을 클릭합니다.

{% hint style="info" %}
**NOTE**\
폴더에 확장자가 pdf, docx, txt, eml인 파일이 있는 경우, 생성형 AI가 언어 처리를 위해 사용하는 벡터 데이터가 자동으로 생성됩니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (414).png" alt="" width="563"><figcaption></figcaption></figure>



4. Guest에게 DirectCloud AI 사용을 허용하려면 ‘게스트 포함’ 항목에 체크합니다.

<figure><img src="../../.gitbook/assets/image (416).png" alt="" width="563"><figcaption></figcaption></figure>



5. EML 파일을 요약하려면 ‘옵션’의 ‘AI 요약’ 항목에 체크합니다.

{% hint style="info" %}
**NOTE**\
‘AI 요약’에 체크하면, 대상 폴더에 확장자가 ‘eml’인 파일을 업로드, 복사 또는 이동할 때 내용이 질문과 답변 형식으로 요약되어 텍스트 파일로 저장됩니다.\
이 요약 처리 과정에서도 토큰 또는 크레딧이 소모됩니다. 또한 요약된 텍스트 파일도 벡터 데이터 생성 대상에 포함됩니다.\
문서의 분량이나 파일 수에 따라 토큰 또는 크레딧이 소모되므로 주의하십시오.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (417).png" alt="" width="563"><figcaption></figcaption></figure>



6. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (418).png" alt="" width="563"><figcaption></figcaption></figure>

‘DirectCloud AI’의 설정이 ‘사용함’으로 변경되면, 폴더의 슬라이드 화면에 ‘DirectCloud AI’ 탭이 생성됩니다.\
또한 ‘폴더 속성’ 탭에서는 ‘폴더 속성’의 ‘버전 관리’ 설정 표시가 사라집니다.\
화면을 새로고침하면 폴더 표시가  <img src="https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000C7Dp&#x26;feoid=00N2w00000JMb2T&#x26;refid=0EMQ80000084aUw" alt="AIフォルダ" data-size="line">  폴더로 변경됩니다.&#x20;

<figure><img src="../../.gitbook/assets/image (419).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**NOTE**\
폴더에 DirectCloud AI가 지원하는 확장자의 파일이 있는 경우, 벡터 데이터 생성이 시작되며 벡터 데이터 생성이 완료된 파일 이름에는 ‘AI’ 아이콘이 표시됩니다.
{% endhint %}
