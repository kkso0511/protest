---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/directcloud-ai/widget
---

# DirectCloud AI의 챗봇 위젯 사용 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용하여 Storage에서 필요한 정보를 빠르게 검색하거나 정보를 요약하기 위한 옵션 서비스인 DirectCloud AI를 제공하고 있습니다.\
Web 브라우저의 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하면, 생성 AI가 대상이 되는 여러 파일을 참조하여 정보를 추출해 제공하는 방식입니다.\
또한 DirectCloud AI에는 전자메일을 파일로 저장할 때 사용되는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 그 내용을 질문과 답변 형식으로 요약하여 텍스트 파일로 저장하는 기능이 있습니다. 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
DirectCloud AI가 활성화된 폴더에서는 목적이나 용도에 따라 여러 개의 채팅룸을 생성할 수 있습니다. 또한 미리 예상되는 질문을 준비하고 특성 등을 설정하여 챗봇으로 활용할 수도 있습니다. 챗봇은 위젯으로 외부 Web사이트에 설정할 수도 있습니다.\
이 매뉴얼에서는, 사용자 페이지에서 DirectCloud AI가 활성화된 폴더에서 챗봇 위젯을 설정하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* DirectCloud의 폴더에서 채팅룸을 이용하는 경우와 챗봇 위젯을 이용하는 경우의 사양 차이 또한 [DirectCloud AI 사양 및 참고 사항](https://help.directcloud.net/user_manual/specification/ai_specification)을 참조해주시기 바랍니다.
* 이 매뉴얼의 절차로 DirectCloud AI를 이용하시려면, 아래 설정이 완료되어 있어야 합니다.
  * [DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/admin_manual/directcloud-ai/enable_ai)의 절차에서 DirectCloud AI를 사용함으로 설정
  * 관리 페이지의 [특정 폴더에 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/admin_manual/directcloud-ai/enable_ai_folder) 또는 [사용자 페이지의 지정된 폴더에서 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/activation)의 절차에서 폴더 속성의 DirectCloud AI를 사용함으로 설정
* 챗봇 위젯을 설정하는 사용자는 <마스터> 권한이 부여되어 있어야 합니다.

***

### 절차

{% hint style="warning" %}
**DirectCloud AI의 채팅룸을 표시하기**
{% endhint %}

챗봇 위젯을 설정하시려면, 사용자 페이지에서 DirectCloud AI가 활성화된 폴더에서 채팅룸을 표시해야 합니다.\
아래의 어느 방법이든 사용하여 DirectCloud AI의 채팅룸을 표시해주시기 바랍니다.

* [DirectCloud AI의 채팅룸을 이용하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/use_chat_room)의 절차에서, DirectCloud AI가 활성화된 폴더의 슬라이드 화면에서 DirectCloud AI 탭을 표시하기
* [DirectCloud AI Home 사용 방법](https://help.directcloud.net/user_manual/directcloud-ai/ai_home)의 절차에서 DirectCloud AI Home을 표시하기



{% hint style="warning" %}
**챗봇 위젯을 설정하기**
{% endhint %}

DirectCloud AI가 활성화된 폴더에는 하나의 챗봇 및 위젯을 설정할 수 있습니다.\
채팅룸 및 챗봇의 기본적인 설정 방법에 대해서는 [DirectCloud AI의 채팅룸을 설정하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/setting_chat_room)을 참조해주시기 바랍니다.<br>

**\[챗봇 위젯 사용을 시작하기]**

1. 설정 버튼을 클릭한 후 위젯을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2338).png" alt=""><figcaption></figcaption></figure>

&#x20;      위젯 화면이 표시됩니다.



2.  위젯을 설정한 후 저장 버튼을 클릭합니다.

    챗봇 위젯 설정이 저장됩니다.<br>

<figure><img src="../../.gitbook/assets/image (2339).png" alt="" width="375"><figcaption></figcaption></figure>

<table><thead><tr><th width="192.5">항목</th><th>내용</th></tr></thead><tbody><tr><td>버튼 이미지</td><td>클릭하면 PC 상의 이미지 파일을 선택하여 챗봇 위젯의 아이콘 이미지를 설정할 수 있습니다.<br>10MB 이하의 JPEG, PNG, GIF 형식의 이미지 파일을 업로드할 수 있습니다.<br>가로세로 비율 1:1(정사각형) 이미지 설정을 권장합니다.</td></tr><tr><td> 세션당 최대 질문 제한</td><td>1회 세션에서 질문할 수 있는 최대 개수를 1~300 사이에서 설정합니다.<br>기본값은 50으로 설정되어 있습니다.</td></tr><tr><td>만료일</td><td>체크하면 챗봇 위젯의 유효 기간을 설정할 수 있습니다.<br>날짜 입력란을 클릭한 후 표시되는 캘린더에서 날짜를 클릭해 유효 기간을 설정할 수 있습니다.</td></tr><tr><td>비밀번</td><td>체크하면 챗봇 위젯을 이용하기 위한 비밀번호를 설정할 수 있습니다.<br>기본값은 8자리 비밀번호가 자동 생성되도록 설정되어 있습니다.<br>챗봇 위젯을 이용하기 위한 비밀번호는 1~32자의 반각 문자로 설정할 수 있으며, 사용할 수 있는 문자 종류와 기호에는 제한이 없습니다.</td></tr></tbody></table>



3. 설정 버튼을 클릭하고, 위젯 메뉴에 이용 중이라고 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2340).png" alt=""><figcaption></figcaption></figure>





**\[챗봇 위젯을 Web페이지에 설치하기]**

1. 위젯 화면에서 위젯의 임베드 코드의 복사 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2341).png" alt="" width="375"><figcaption></figcaption></figure>



2. 복사한 임베드 코드를 챗봇 위젯을 설치하려는 Web 페이지에 삽입합니다

{% hint style="info" %}
**NOTE:**\
위젯은 여러 Web페이지에 삽입할 수 있습니다.
{% endhint %}



3. Web 페이지에 챗봇 위젯 아이콘이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2343).png" alt=""><figcaption></figcaption></figure>

\
**\[챗봇 위젯 사용 중지하기]**

챗봇 위젯 사용을 중지하려면 사용 중인 위젯을 삭제해야 합니다.\
위젯을 삭제하면, 위젯 임베드 코드에 포함된 data-widget-id가 무효화됩니다. 또한, 위젯 임베드 코드가 삽입된 Web페이지를 다시 로드하면 위젯 표시가 사라집니다.

1. 위젯 화면에서 위젯 삭제 버튼을 클릭합니다.

{% hint style="info" %}
**NOTE:**\
여러 Web페이지에 위젯을 설치한 경우, 모든 Web페이지에서 챗봇 위젯을 사용할 수 없게 되므로 주의해주시기 바랍니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2342).png" alt="" width="375"><figcaption></figcaption></figure>



2. Web페이지에 챗봇 위젯이 설치되어 있는 경우, 삭제 확인 화면이 표시됩니다.\
   '삭제' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2344).png" alt="" width="375"><figcaption></figcaption></figure>



{% hint style="warning" %}
**챗봇 위젯 이용하기**
{% endhint %}

1. 챗봇 위젯을 설치한 Web페이지를 표시한 후, 위젯 아이콘을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2345).png" alt=""><figcaption></figcaption></figure>



2. 챗봇 위젯에 비밀번호가 설정되어 있는 경우, 비밀번호를 입력한 후 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2346).png" alt=""><figcaption></figcaption></figure>



3. DirectCloud의 채팅룸과 동일한 방식으로 DirectCloud AI에 질문합니다.\
   자세한 내용은 [DirectCloud AI의 채팅룸을 이용하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/use_chat_room)을 참조해주시기 바랍니다.

<figure><img src="../../.gitbook/assets/image (2347).png" alt=""><figcaption></figcaption></figure>
