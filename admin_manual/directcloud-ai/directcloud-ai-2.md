---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-ai/directcloud-ai-2
---

# DirectCloud AI 대화 로그를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성 AI를 활용해 Storage에서 필요한 정보를 빠르게 찾아낼 수 있는 옵션 서비스인 DirectCloud AI를 제공하고 있습니다.\
사용자 페이지에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하시면, 생성 AI가 대상이 되는 여러 파일을 검색하여 정보를 추출해 제공합니다.\
또한 DirectCloud AI에는 전자메일을 파일로 저장할 때 사용하는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 내용을 질문과 답변 형식으로 요약해 텍스트 파일로 저장하는 기능이 있습니다. 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참고됩니다.\
이 매뉴얼에서는 관리자 페이지의 DirectCloud AI > 대화 로그에서 사용자가 채팅룸에서 질문한 내용과 DirectCloud AI가 제공한 답변을 로그로 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* DirectCloud AI에 공통되는 사양 및 주의 사항에 대해서는 [DirectCloud AI 사양 및 참고사항](https://help.directcloud.net/user_manual/undefined-14/directcloud-ai)을 참조해 주시기 바랍니다.
* 내보내기되는 텍스트 파일의 문자 인코딩은 '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩' 설정에서 지정됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**대화 로그 보기**
{% endhint %}

**\['채팅 로그' 화면에서 '폴더'를 선택하기]**

1. 'DirectCloud AI' > '대화 로그' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>



2. 폴더 영역에서 대화 로그의 내용을 확인할 폴더를 선택합니다.\
   채팅방 목록은 마지막 사용 순서대로 위에서 표시됩니다.

{% hint style="info" %}
**NOTE**\
폴더 영역에 표시되는 폴더는 계층 구조가 아니라 병렬로 표시됩니다. 실제 공유 메뉴의 폴더 구성과는 다릅니다.\
과거에 DirectCloud AI가 활성화로 설정되어 있었던 폴더는 연한 회색으로 표시됩니다. 클릭하면 해당 폴더의 채팅 로그를 확인할 수 있습니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

**\[폴더의 채팅 로그를 확인하기]**

대상 폴더의 채팅방을 선택하여 채팅 로그를 확인합니다.

1. '폴더' 탭에서, 폴더에서 생성된 채팅방 목록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="164.5">항목</th><th>설명</th></tr></thead><tbody><tr><td>대화명</td><td>채팅방의 이름이 표시됩니다.</td></tr><tr><td>사용자</td><td>채팅방을 생성한 사용자의 이름이 표시됩니다.</td></tr><tr><td>대화 시작 일시</td><td>DirectCloud AI의 채팅방에서 채팅을 시작한 일시가 표시됩니다.</td></tr><tr><td>최근 대화 일시</td><td>DirectCloud AI의 채팅방에서 채팅을 종료한 일시가 표시됩니다.</td></tr><tr><td>내역</td><td>상세 표시 버튼이 표시됩니다.</td></tr></tbody></table>



2. 채팅 로그를 확인하려는 채팅방의 '상세' 항목에 표시된 상세 표시 버튼을 클릭합니다.

{% hint style="info" %}
**NOTE**\
사용자 페이지에서 채팅룸 이름이 변경되면 채팅룸명에 표시되는 이름도 함께 변경됩니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (2566).png" alt=""><figcaption></figcaption></figure>

&#x20;  채팅 기록 화면에는 채팅룸에서 입력한 질문과 답변 로그가 새로운 순서대로 위에서부터 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2567).png" alt="" width="563"><figcaption></figcaption></figure>



**\[챗봇 위젯의 채팅 로그를 확인하기]**

대상 폴더에서 생성된 챗봇을 선택하여, 챗봇 위젯의 채팅 로그를 확인합니다.

1. '챗봇위젯' 탭에서, 챗봇 로그의 목록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2569).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="164.5">항목</th><th>설명</th></tr></thead><tbody><tr><td>챗봇명</td><td>챗봇의 이름이 표시됩니다.</td></tr><tr><td>사용자</td><td>챗봇 위젯을 이용한 사용자에게 자동으로 할당되는 고유한 값이 표시됩니다.</td></tr><tr><td>진입 경로</td><td>챗봇 위젯을 실행한 경로를 표시합니다.</td></tr><tr><td>대화시작 일시</td><td>챗봇 위젯에서 채팅을 시작한 일시가 표시됩니다.</td></tr><tr><td>최근 대화 일시</td><td>챗봇 위젯에서 채팅을 종료한 일시가 표시됩니다.</td></tr><tr><td>내역</td><td>상세 표시 버튼이 표시됩니다.</td></tr></tbody></table>



2. 채팅 로그를 확인하려는 챗봇의 '내역' 항목에 표시된 상세 표시 버튼을 클릭합니다.

{% hint style="info" %}
**NOTE**\
사용자 페이지에서 채팅방 이름이 변경되면, '채팅방 이름'에 표시된 이름도 변경됩니다.
{% endhint %}



<figure><img src="../../.gitbook/assets/image (2570).png" alt=""><figcaption></figcaption></figure>

'채팅 이력' 화면에는 챗봇 위젯에서 입력한 질문과 답변의 로그가, 새로운 로그가 위에서부터 순서대로 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2571).png" alt="" width="563"><figcaption></figcaption></figure>





{% hint style="warning" %}
**대화 로그 다운로드**
{% endhint %}

대화 로그 화면에 표시된 대화 내역은 기간을 지정해 텍스트 파일로 다운로드할 수 있습니다.

1. 대화 내역 화면에서 '채팅 다운로드'를 클릭합니다.\
   다운로드 설정이 표시됩니다.\
   채팅다운로드 버튼을 다시 클릭하면 다운로드 설정을 닫을 수 있습니다.

<figure><img src="../../.gitbook/assets/image (337).png" alt=""><figcaption></figcaption></figure>



2. 다운로드하려는 대화 로그의 기간을 지정한 뒤 txt 다운로드 버튼을 클릭합니다.\
   지정한 기간의 대화 로그가 텍스트 파일로 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (339).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="99.60003662109375">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>계약 시작부터 현재까지의 DirectCloud AI 대화 로그를 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 최대 12개월입니다.</td></tr><tr><td>2</td><td>DirectCloud AI의 대화 로그를 표시할 기간을 최근 7일, 최근 15일, 최근 1개월, 최근 3개월 중에서 선택합니다.</td></tr></tbody></table>



3. 다운로드한 텍스트 파일을 열어 대화 로그가 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (340).png" alt=""><figcaption></figcaption></figure>
