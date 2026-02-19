---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/directcloud-ai/file_preparation
---

# DirectCloud AI를 활용하기 위한 파일을 준비하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 생성형 AI를 활용하여 스토리지에서 필요한 정보를 빠르게 찾아내거나 요약할 수 있는 옵션 서비스인 DirectCloud AI를 제공합니다.\
Web 브라우저에서 DirectCloud AI가 활성화된 폴더에서 채팅을 시작하고 궁금한 점을 입력하면, 생성형 AI가 해당 폴더 내 여러 파일을 참조하여 관련 정보를 추출해 제시하는 구조입니다.\
또한 DirectCloud AI에는 이메일을 파일로 저장할 때 사용되는 파일 형식인 EML 파일을 EML 요약이 활성화된 폴더에 업로드하면, 내용을 질문과 답변 형식으로 요약해 텍스트 파일로 저장하는 기능이 있습니다. 이 요약된 텍스트 파일도 DirectCloud AI의 채팅에서 참조됩니다.\
이 매뉴얼에서는 DirectCloud AI를 사용하기 전에, DirectCloud AI가 활성화된 폴더에 처리 대상 파일을 업로드하여 준비하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 사용자 페이지의 폴더 속성에서 DirectCloud AI 설정을 수행하는 사용자에게는 <마스터> 권한이 설정되어 있어야 합니다.
* ‘DirectCloud AI’ 설정은 기본적으로 ‘사용하지 않음’으로 설정되어 있습니다.
* 이 매뉴얼의 설정을 진행 하려면 먼저관리 페이지의 ‘DirectCloud AI’ > ‘설정’ 메뉴에서 ‘사용’을 선택해야 합니다.
* ‘DirectCloud AI'가 ‘사용함’으로 설정된 폴더가 있는 경우, 관리 페이지의 ‘DirectCloud AI’ > ‘설정’ 메뉴에서 ‘사용 안함’을 선택할 수 없습니다.
*   Web 애플리케이션에서 DirectCloud AI를 사용하기 위한 파일을 준비하는 방법에는 다음 두 가지가 있습니다.

    1. 폴더 트리에서 DirectCloud AI가 활성화된 폴더를 표시하는 방법
    2. DirectCloud AI Home을 표시하는 방법

    이 매뉴얼에서는 DirectCloud AI가 활성화된 폴더의 슬라이드 화면을 사용하여 설명하고 있습니다.\
    DirectCloud AI Home에서도 ‘대상 파일 목록’ 영역에 파일을 업로드하면 벡터 데이터를 생성할 수 있습니다.\
    단, ‘텍스트 추출 중’ 등의 처리 상태를 나타내는 문구나 벡터 데이터가 생성되었음을 나타내는 ‘AI’ 라벨은 표시되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. DirectCloud AI를 사용하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2222).png" alt=""><figcaption></figcaption></figure>



2. 폴더의 슬라이드 화면에서 'DirectCloud AI'가 '사용'으로 설정되어 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2221).png" alt=""><figcaption></figcaption></figure>



3. 업로드가 완료되면, DirectCloud AI가 언어 처리를 위해 사용하는 벡터 데이터 생성이 시작됩니다.\
   벡터 데이터 처리에는 몇 분이 소요될 수 있습니다.\
   처리 내용은 폴더 속성의 ‘DirectCloud AI’ 설정에서 ‘AI 요약’ 항목이 체크되어 있는지 여부에 따라 달라집니다.

* ‘AI 요약’ 항목에 체크되어 있지 않은 경우:\
  처리 중인 파일에는 처리 상태에 따라 해당 내용이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2223).png" alt=""><figcaption></figcaption></figure>

| 텍스트         | 설명                                  |
| ----------- | ----------------------------------- |
| 텍스트 추출 중    | 업로드, 복사 또는 이동된 파일에서 텍스트를 추출하고 있습니다. |
| 벡터 데이터 생성 중 | 추출된 텍스트의 벡터 데이터를 생성하고 있습니다.         |

벡터 데이터 생성이 완료된 파일 이름에는 ‘AI’ 아이콘이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2224).png" alt=""><figcaption></figcaption></figure>

* ‘AI 요약’ 항목에 체크되어 있는 경우, 처리 중인 파일에는 처리 상태에 따라 해당 내용이 표시됩니다.\
  벡터 데이터 생성이 완료된 파일 이름에는 ‘AI’ 아이콘이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2226).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="178.5">텍스트</th><th>설명</th></tr></thead><tbody><tr><td>텍스트 추출 중</td><td>업로드, 복사 또는 이동된 EML 파일에서 텍스트를 추출하고 있습니다.</td></tr><tr><td>요약 중</td><td>EML 파일의 내용을 질문과 답변 형식으로 요약하고 있습니다.<br>요약된 내용은 텍스트 파일로 저장됩니다.</td></tr><tr><td>벡터 데이터 생성 중</td><td>요약된 텍스트 파일의 벡터 데이터를 생성하고 있습니다.</td></tr></tbody></table>

요약된 내용은 원본 파일 이름에 확장자 ‘txt’가 추가된 텍스트 파일로 저장됩니다.\
원본 EML 파일은 ‘EML’ 폴더로 이동되며, ‘EML’ 폴더가 존재하지 않는 경우 자동으로 생성됩니다.

<figure><img src="../../.gitbook/assets/image (2225).png" alt=""><figcaption></figcaption></figure>
