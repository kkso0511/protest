---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/directcloud-ai/data_chunk
---

# DirectCloud AI의 데이터 청크를 편집하는 방법

### 개요

DirectCloud에서는 생성 AI를 활용하여 Storage 내에서 필요한 정보를 빠르게 검색하거나 요약할 수 있는 옵션 서비스인 DirectCloud AI를 제공합니다.\
Web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 알고 싶은 내용을 질문하면, 생성 AI가 해당 폴더의 여러 파일을 참조하여 관련 정보를 추출하고 제공합니다.\
또한 DirectCloud AI에는 이메일을 파일로 저장할 때 사용하는 파일 형식인 EML 파일을, EML 요약이 활성화된 폴더에 업로드하면 내용을 질문과 답변 형식으로 요약하여 텍스트 파일로 저장하는 기능이 있습니다.\
이렇게 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
DirectCloud AI가 추출한 데이터는 ‘데이터 청크’라는 작은 단위의 텍스트 데이터로 분할되어 저장됩니다.\
데이터 청크를 편집하면 DirectCloud AI의 채팅에서 의도한 대로 더 정확한 답변을 받을 수 있습니다.\
이 매뉴얼에서는 DirectCloud AI가 추출한 데이터 청크를 편집하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼의 절차를 따라 DirectCloud AI를 사용하려면 다음 설정이 완료되어 있어야 합니다.
  * 관리자 페이지의 'DirectCloud AI'->'설정' 에서 DirectCloud AI 를 '사용' 으로 설정
  * 폴더 속성의 ‘DirectCloud AI’를 ‘사용함’으로 설정
  * [DirectCloud AI를 사용하기 위한 파일을 준비하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/directcloud-ai-1) 절차에 따라 DirectCloud AI의 처리 대상 파일 준비 완료
* Web 브라우저에서 DirectCloud AI를 사용하는 방법은 다음 두 가지입니다.
  1. [사용자 페이지의 지정된 폴더에서 DirectCloud AI를 활성화하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/directcloud-ai)에 따라 DirectCloud AI가 활성화된 폴더의 슬라이드 화면에서 ‘DirectCloud AI’ 탭을 표시하는 방법
  2. DirectCloud AI Home을 표시하는 방법
* 데이터 청크를 편집하려면 <마스터> 권한 또는 <전체권한>, <편집자>, <편집자-> 접근 권한이 부여되어 있어야 합니다.

***

### 절차

{% hint style="warning" %}
**데이터 청크 편집 화면 표시하기**
{% endhint %}

**\[DirectCloud AI가 활성화된 폴더에서 표시합니다]**

1. Shared Box에서 DirectCloud AI가 활성화된 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (388).png" alt=""><figcaption></figcaption></figure>



2. 다음 중 하나의 방법으로 데이터 청크 편집 화면을 표시합니다.

❶ 데이터 청크를 편집하려는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 ‘AI 데이터 관리’를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (389).png" alt=""><figcaption></figcaption></figure>

❷ 데이터를 편집하려는 파일의 오른쪽에 있는 ▼ 버튼을 클릭하고, 표시된 메뉴에서 ‘AI 데이터 관리’를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (390).png" alt=""><figcaption></figcaption></figure>



**\[DirectCloud AI Home에서 표시하기]**

1. DirectCloud AI Home을 표시하고 사용할 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (392).png" alt=""><figcaption></figcaption></figure>



2. ‘파일 목록’에서 데이터 청크를 편집하려는 파일의 오른쪽에 표시된 버튼을 클릭합니다.\
   데이터 편집 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (391).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**데이터 청크 편집하기**
{% endhint %}

**\[데이터 청크 편집 화면의 구성]**

<figure><img src="../../.gitbook/assets/image (393).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="119.4000244140625">No.</th><th width="200.4000244140625">설정항목</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>데이터 청크 목록</td><td>현재 선택된 페이지의 데이터 청크가 최대 20개까지 표시됩니다. 각 데이터 청크에는 순번이 부여됩니다. 데이터 청크 번호 뒤에는 추출된 원본 파일의 페이지 정보와 추출된 텍스트의 첫 부분이 표시됩니다. 단, 원본 파일에 페이지가 없는 경우(텍스트 파일, EML 파일 등)는 페이지 정보가 표시되지 않습니다. 목록에서 데이터 청크를 클릭하면 ❸에 해당 청크의 상세 정보가 표시됩니다.</td></tr><tr><td>❷</td><td>데이터 청크 수</td><td>❻에서 현재 선택된 페이지의 데이터 청크 수가 표시됩니다.</td></tr><tr><td>❸</td><td>데이터 청크 표시 영역</td><td>각 데이터 청크의 헤더 행에는 추출된 데이터 청크의 글자 수와 원본 파일의 페이지 정보가 표시됩니다. 두 번째 행부터는 추출된 데이터 청크의 텍스트가 표시되며, 여기서 직접 텍스트를 편집할 수 있습니다. 텍스트를 편집하면 해당 청크에 ‘수정’ 배지가 표시됩니다. 각 데이터 청크의 최대 입력 가능 글자 수는 1500자이며, 텍스트를 모두 삭제하면 ❼의 ‘저장’ 버튼을 클릭할 수 없습니다. 화면을 위아래로 스크롤하여 페이지 내 청크를 이동할 수 있습니다.</td></tr><tr><td>❹</td><td>삭제</td><td>클릭하면 삭제할 청크에 ‘삭제’ 배지가 표시됩니다. 실제 삭제는 ❼의 ‘저장’ 버튼을 클릭했을 때 이루어집니다. 모든 데이터 청크를 삭제하면 ❼에서 ‘저장’ 버튼을 클릭할 수 없습니다. 최소 한 개의 데이터 청크가 필요합니다.</td></tr><tr><td>❺</td><td>데이터 청크 번호</td><td>현재 ❶에 표시된 데이터 청크 번호 범위 / 전체 데이터 청크 수가 표시됩니다.</td></tr><tr><td>❻</td><td>페이지 표시/선택</td><td>추출된 데이터 청크의 전체 페이지 수가 표시되며, 현재 표시 중인 페이지 번호는 파란색으로 표시됩니다. 번호를 클릭하면 해당 페이지로 이동할 수 있습니다.</td></tr><tr><td>❼</td><td>저장</td><td>클릭하면 데이터 청크의 편집 내용이 저장됩니다. ❻에서 페이지를 이동하기 전에 반드시 편집 내용을 저장해야 합니다. 저장에 실패한 경우, 해당 청크에 표시된 ‘삭제’, ‘수정’ 배지가 그대로 남습니다. 이때 해당 청크를 수정한 후 다시 저장해야 합니다.</td></tr><tr><td>❽</td><td>닫기</td><td>클릭하면 데이터 청크 편집 화면이 닫힙니다. 저장되지 않은 편집 내용이 있을 경우, 클릭 시 변경 내용이 취소되고 편집 화면이 닫힙니다.</td></tr></tbody></table>



**\[데이터 청크 편집하기]**

1. 왼쪽의 데이터 청크 목록에서 데이터 청크 번호를 클릭하거나, 오른쪽에 표시된 데이터 청크 영역을 스크롤하여 편집하려는 데이터 청크를 표시합니다.

<figure><img src="../../.gitbook/assets/image (394).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**NOTE**\
데이터 청크는 페이지 단위로 편집됩니다. 오른쪽 아래의 번호를 클릭하면 페이지를 이동할 수 있습니다.\
단, 저장되지 않은 편집 내용이 있는 경우에는 아래와 같은 대화상자가 표시됩니다. ‘저장 후 이동’ 버튼을 클릭하면 편집 내용이 저장된 후 지정한 페이지로 이동합니다.
{% endhint %}



2. 데이터 청크의 내용을 변경하려면 데이터 청크 표시 영역에서 직접 텍스트를 편집합니다.\
   편집을 하면 데이터 청크 목록에 즉시 ‘수정’ 배지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (395).png" alt=""><figcaption></figcaption></figure>



3. 특정 데이터 청크를 삭제하려면 해당 데이터 청크의 ‘삭제’ 버튼을 클릭합니다.\
   데이터 청크 목록에 ‘삭제’ 배지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (396).png" alt=""><figcaption></figcaption></figure>



4. 삭제한 데이터 청크를 되돌리려면, 데이터 청크 오른쪽 상단에 표시된 ‘삭제 취소’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (397).png" alt=""><figcaption></figcaption></figure>



**\[편집한 데이터 청크를 저장]**

1. 편집한 데이터 청크를 저장하려면, 오른쪽 상단에 표시된 ‘저장’ 버튼을 클릭합니다.

{% hint style="info" %}
**NOTE**\
편집 내용이 있는 상태에서 ‘닫기’를 클릭하면, 편집한 내용이 저장되지 않고 취소되며 데이터 청크 편집 화면이 닫힙니다.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (398).png" alt=""><figcaption></figcaption></figure>

데이터 청크의 편집 내용이 반영되며, ‘수정’ 및 ‘삭제’ 표시가 사라집니다.

<figure><img src="../../.gitbook/assets/image (399).png" alt=""><figcaption></figcaption></figure>



2. 데이터 청크 편집 화면을 닫으려면, 오른쪽 상단에 표시된 ‘닫기’ 버튼을 클릭합니다.
