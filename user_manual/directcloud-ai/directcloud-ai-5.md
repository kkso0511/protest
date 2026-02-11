---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/directcloud-ai/directcloud-ai-5
---

# DirectCloud AI 오류 메시지를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용하여 Storage 내에서 필요한 정보를 빠르게 검색하거나 요약할 수 있는 옵션 서비스인 DirectCloud AI를 제공합니다.\
Web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하면, 생성 AI가 해당 폴더 내 여러 파일을 참조하여 관련 정보를 추출하고 제공합니다.\
또한 DirectCloud AI에는 이메일을 파일로 저장할 때 사용하는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 내용을 질문과 답변 형식으로 요약하여 텍스트 파일로 저장하는 기능이 있습니다.\
이렇게 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
이 매뉴얼에서는 사용자 페이지에서 DirectCloud AI를 이용할 때 표시되는 오류 메시지에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼의 절차를 따라 DirectCloud AI를 사용하려면 다음 설정이 완료되어 있어야 합니다.
  * 관리자 페이지의 'DirectCloud AI'->'설정' 에서 DirectCloud AI 를 '사용' 으로 설정
  * 폴더 속성의 ‘DirectCloud AI’를 ‘사용함’으로 설정
  * [DirectCloud AI를 사용하기 위한 파일을 준비하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/directcloud-ai-1) 절차에 따라 DirectCloud AI의 처리 대상 파일 준비 완료
*   Web 브라우저에서 DirectCloud AI를 사용하는 방법은 다음 두 가지입니다.

    1. [사용자 페이지의 지정된 폴더에서 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/directcloud-ai)에 따라 DirectCloud AI가 활성화된 폴더의 슬라이드 화면에서 ‘DirectCloud AI’ 탭을 표시하는 방법
    2. DirectCloud AI Home을 표시하는 방법

    이 매뉴얼 에서는 폴더 목록 중 DirectCloud AI가 활성화된 폴더를 사용하는 예시로 설명합니다.\
    DirectCloud AI Home의 ‘파일 목록’ 영역에는 ‘텍스트 추출 중’ 등의 처리 상태 메시지나, 벡터 데이터가 생성되었음을 나타내는 ‘AI’ 라벨, 또는 처리 실패 시의 실패 아이콘이 표시되지 않습니다.\
    따라서, 이 매뉴얼의 절차를 통해 파일 목록의 오류를 확인할 수는 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**파일 목록 오류 확인**
{% endhint %}

파일을 업로드하거나 DirectCloud AI를 활성화할 때 벡터 데이터를 만들지 못하면 파일 목록에 실패 아이콘 <img src="https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001BcX&#x26;feoid=00N2w00000JMb2T&#x26;refid=0EMQ800000413WE" alt="ic_failed.png" data-size="line"> 이표시됩니다. 아이콘을 클릭하면 오류 메시지가 표시됩니다.

{% hint style="info" %}
**NOTE**: 접근 권한이 업로더인 사용자는 DirectCloud AI를 사용할 수 없기 때문에, 벡터 데이터 생성에 실패하더라도 파일 목록에는 실패 아이콘이 표시되지 않습니다.
{% endhint %}



**\[오류 메시지 표시 절차]**

1. DirectCloud AI 오류를 확인할 폴더를 클릭합니다.
2. 파일 목록에 표시되는  <img src="https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001BcX&#x26;feoid=00N2w00000JMb2T&#x26;refid=0EMQ800000413WE" alt="ic_failed.png" data-size="line"> 아이콘을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001BcX\&feoid=00N2w00000JMb2T\&refid=0EMQ80000040hQr)

오류 메시지가 표시됩니다.

벡터 데이터를 생성할 수 있는 파일의 경우, 오류 메시지 확인 화면에 ‘재실행’ 버튼과 ‘닫기’ 버튼이 표시됩니다. ‘재실행’ 버튼을 클릭하면 벡터 데이터 생성이 다시 시작됩니다.\
알 수 없는 오류로 인해 벡터 데이터 생성에 실패한 경우, 오류 메시지 확인 화면에\
“DirectCloud AI 사용을 위한 데이터 준비에 실패하였습니다. 다시 시도하시겠습니까?”\
라는 메시지가 표시됩니다.\
‘확인’ 버튼을 클릭하면 벡터 데이터 생성이 다시 시작됩니다.

{% hint style="info" %}
**NOTE**\
데이터 청크 생성에 실패한 파일이 있는 경우, 폴더를 표시할 때 몇 초 동안 폴더 및 파일 목록 상단에\
“데이터 청크 생성에 실패한 파일이 있습니다.”\
라는 메시지가 표시됩니다.\
‘재실행’ 버튼을 클릭하면 데이터 청크 생성을 다시 요청할 수 있습니다.
{% endhint %}



**\[파일 목록 오류 메시지]**

| 오류 메세지                                                                                                        | 설명                                                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 암호가 있는 파일입니다. 암호 해제 후 다시 업로드해 주세요.                                                                            | <p>비밀번호로 암호화된 PDF 파일을 업로드하면 벡터 데이터 작성이 실패합니다.<br>이 오류의 경우 오류 메시지 확인 화면에 "재실행" 버튼이 표시되지 않습니다.</p>                                                                 |
| 파일에 암호가 걸려있거나 파일이 손상이 되었습니다.                                                                                  | <p>암호로 암호화된 Word 파일(확장자 docx)을 업로드하면 벡터 데이터를 만들지 못합니다.<br>암호화된 파일과 손상된 파일은 구별할 수 없습니다.<br>이 오류의 경우 오류 메시지 확인 화면에 "재실행" 버튼이 표시되지 않습니다.</p>                        |
| 관리자페이지에 등록한 Azure OpenAl Service 설정 정보(API Key, API URI, Deployment Name)가 유효하지 않습니다. 유효한 정보 입력 후 다시 시도해 주세요. | <p>입력한 Azure OpenAI Service 설정이 유효하지 않으면 벡터 데이터를 만들지 못합니다.<br>오류 메시지 확인 화면에서 "재실행" 버튼을 클릭하면 벡터 데이터 생성을 다시 실행할 수 있습니다.</p>                                        |
| 분당 토큰 속도 제한을 초과했거나 할당된 토큰 부족으로 요청을 처리할 수 없습니다.                                                                | <p>Azure OpenAI Service에서 결정한 분당 사용 가능한 토큰 수 또는 월간 할당량을 초과하면 내부 오류 105에서 벡터 데이터를 만들지 못합니다.<br>오류 메시지 확인 화면에서 "재실행" 버튼을 클릭하면 벡터 데이터 생성을 다시 실행할 수 있습니다.</p>        |
| Azure OpenAI Service에서 서버와 통신 중 오류 응답을 받았습니다. 잠시 후 다시 시도해 주세요.                                                | <p>Azure OpenAI Service 서버 오류 500이 발생하면 내부 오류 106에서 벡터 데이터를 만들지 못합니다.<br>오류 메시지 확인 화면에서 "재실행" 버튼을 클릭하면 벡터 데이터 생성을 다시 실행할 수 있습니다.</p>                             |
| Azure OpenAI Service에서 서버 과부하 응답을 받았습니다. 잠시 후 다시 시도해 주세요.                                                     | <p>Azure OpenAI Service의 서버 오류 503이 발생하면 Azure OpenAI 서버에 대한 부하로 인해 내부 오류 107에서 벡터 데이터를 만들지 못합니다.<br>오류 메시지 확인 화면에서 "재실행" 버튼을 클릭하면 벡터 데이터 생성을 다시 실행할 수 있습니다.</p> |
| DirectCloud AI 사용을 위한 데이터 준비에 실패하였습니다. 다시 시도하시겠습니까?                                                           | <p>알 수 없는 오류로 벡터 데이터를 만들지 못했습니다.<br>에러 메시지 확인 화면에서 [OK] 버튼을 클릭하면 다시 벡터 데이터 작성을 실행할 수 있습니다.</p>                                                                   |



{% hint style="warning" %}
**'DirectCloud AI' 채팅 오류 메시지 확인**
{% endhint %}

토큰 부족이나 질문·답변 관련 오류가 발생한 경우, DirectCloud AI 채팅의 질문 또는 답변 영역에 오류 메시지가 표시됩니다.

{% hint style="info" %}
**NOTE**\
DirectCloud AI 채팅에서 질문을 입력할 때 입력 가능한 토큰 수를 초과하면, 그 이상 문자를 입력할 수 없습니다. 이 경우에는 오류 메시지가 표시되지 않습니다.
{% endhint %}



**\[오류 메시지 표시 절차]**

1. DirectCloud AI 채팅을 표시합니다.\
   질문이나 답변에 표시되는 오류 메시지를 확인합니다.

<figure><img src="../../.gitbook/assets/image (387).png" alt=""><figcaption></figcaption></figure>



**\['DirectCloud AI' 채팅 오류 메시지]**

<table><thead><tr><th width="318.79998779296875">오류 메세지</th><th>설명</th></tr></thead><tbody><tr><td>폴더에 파일이 없습니다. 먼저 파일을 업로드해 주세요.</td><td>DirectCloud AI가 활성화된 폴더에 파일이 없는 상태에서 질문을 입력하면 오류 메시지가 표시됩니다.</td></tr><tr><td>DirectCloud AI 사용을 위한 데이터 준비 중입니다. 잠시 후 다시 시도해 주세요.</td><td>질문을 입력할 때 벡터 데이터가 생성된 파일이 없으면 답변에 오류 메시지가 표시됩니다.</td></tr><tr><td>답변 가능한 글자수를 초과하여 일부 내용을 수신하지 못했습니다.</td><td>응답 가능한 최대 토큰 수를 초과한 경우 내부 오류 110이 발생합니다.<br>이때 출력 가능한 부분까지의 답변이 표시된 후, 문장 끝의 괄호 안에 오류 메시지가 함께 표시됩니다.</td></tr><tr><td>Microsoft OpenAI Service의 제한에 걸려 사용할 수 없습니다. 관리자에게 문의하십시오.</td><td>Azure OpenAI Service에서 결정한 분당 사용 가능한 토큰 수 또는 월 할당량을 초과하면 내부 오류 105가 발생합니다.<br>질문이나 답변에 오류 메시지가 표시됩니다.</td></tr><tr><td>알 수 없는 에러가 발생했습니다. 잠시 후에 다시 이용해 주세요.</td><td>위의 내용에 해당하지 않는 오류가 발생하면 내부 오류 114입니다.<br>해당 질문 또는 답변에 오류 메시지가 표시됩니다.</td></tr></tbody></table>
