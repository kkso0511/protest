---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-3/undefined
---

# 파일을 다운로드하지 않고 온라인으로 편집하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 파일을 다운로드하지 않고 전용 응용 프로그램에서 온라인으로 편집하는 방법에 대해 설명합니다.

***

### 동작조건

* 본 매뉴얼의 절차에서는 Shared Box에서의 작업 방법을 설명하고 있지만, Connect 폴더와 DLP 폴더도 동일한 절차로 작업할 수 있습니다.
* 다음 폴더에 저장된 파일은 온라인으로 편집할 수 없습니다.
  * DirectCloud AI가 사용 가능한 폴더
  * Warm Storage 폴더
  * Cold Storage 폴더
* 온라인 편집을 수행하려면 관리자 페이지에서 온라인 편집 기능을 사용하도록 설정해야 합니다.
* 온라인 편집을 위해서는 '마스터', '전체권한', '편집자', '편집자'의 접근 권한이 부여되어 있어야 합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 온라인 편집에서는 100MB 이하의 파일을 최대 5명이 동시에 편집할 수 있습니다.
* 온라인 편집으로 편집한 내용은 모든 사용자가 편집 화면을 닫았을 때 저장됩니다.
* Microsoft Office가 설치되어 있지 않은 PC에서도 Office 파일을 편집할 수 있습니다.\
  온라인 편집을 지원하는 확장자는 다음과 같습니다.\
  .xls, .xlsx, .doc, .docx, .ppt, .pptx
* DirectCloud-SHIELD IRM으로 암호화된 파일도 위 확장자의 파일이라면 온라인 편집 및 댓글 추가가 가능합니다.
* 구형 Office 파일(.doc, .ppt, .xls)을 온라인 편집할 경우, 편집 화면에 표시하려면 신형 Office 파일(.docx, .pptx, .xlsx)로 변환할 것인지 확인하는 다이얼로그에서 ‘OK’ 버튼을 클릭해야 합니다.
* 텍스트 파일이나 매크로 파일은 온라인 편집할 수 없습니다.
* DirectCloud Drive에서는 DirectCloud 전용 애플리케이션이 아니라 Microsoft Office 애플리케이션으로 직접 편집할 수도 있습니다.
* 온라인 편집 세션 시간은 30일입니다.
* 여러 웹 브라우저를 사용하여 여러 파일을 동시에 편집할 수 있지만, 파일 간 데이터를 복사할 수는 없습니다.
*   관리 페이지의 ‘로그 현황’ > ‘파일 이용 내역’ 메뉴에는 다음 시점에 온라인 편집 작업 로그가 기록됩니다.

    * 온라인 편집
    * 온라인 편집 화면을 실행했을 때
    * 덮어쓰기 저장, 즉 파일 내용을 변경하고 온라인 편집 화면을 종료했을 때

    파일 편집 중 저장한 시점에서는 로그가 기록되지 않습니다. 또한, 파일 내용을 변경하지 않고 편집 화면을 종료하거나 댓글만 추가했을 때도 로그가 기록되지 않습니다.
* 온라인 편집한 파일의 내용을 저장하지 않고 닫을 수 없습니다.\
  관리 페이지 설정에서도 온라인 편집 파일을 저장하지 않도록 설정할 수 없습니다.\
  편집 이전의 파일로 되돌리는 방법은 [파일 버전을 복원하는 방법](https://help.directcloud.net/user_manual/undefined-3/undefined-1)을 참고해주시기 바랍니다.
* 온라인 편집 화면에서 표시된 파일은 인쇄할 수 없습니다.
* Office 파일에 댓글을 추가한 경우, 표시되는 사용자 이름은 다음과 같습니다.
  * 온라인 편집에서 댓글 추가: DirectCloud 사용자 이름
  * Microsoft Office에서 댓글 추가: Microsoft Office 계정 이름
* 온라인 편집 화면이 표시되는 데 시간이 걸릴 경우, 웹 브라우저 캐시를 삭제한 후 다시 시도하십시오.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 온라인 편집 화면 열기**
{% endhint %}

1. 온라인 편집할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1380).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나로 온라인 편집 화면을 표시합니다.

&#x20;     ❶  편집하고 싶은 파일을 체크하고 상단의 '편집' 버튼을 클릭

<figure><img src="../../.gitbook/assets/image (1381).png" alt=""><figcaption></figcaption></figure>

&#x20;      ❷  편집할 파일을 마우스 오른쪽 버튼으로 클릭하고 "편집"을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1382).png" alt=""><figcaption></figcaption></figure>

&#x20;       ❸  편집하고자 하는 파일의 오른쪽에 있는 ▼ 버튼을 클릭하고 표시된 메뉴에서 '편집'을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1383).png" alt=""><figcaption></figcaption></figure>

&#x20;      ❹  파일을 클릭하여 미리보기 화면을 표시하고 오른쪽 상단의 '편집' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1384).png" alt=""><figcaption></figcaption></figure>

&#x20;      온라인 편집 화면이 표시됩니다.



3. 파일을 편집할 수 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1385).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 온라인 편집 화면 열기**
{% endhint %}

1. 탐색기에서 편집할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1386).png" alt=""><figcaption></figcaption></figure>



2. 편집할 파일을 오른쪽 마우스로 클릭하고 'DirectCloud-Drive' > '문서편집'을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1387).png" alt=""><figcaption></figcaption></figure>

&#x20;      DirectCloud 전용 애플리케이션이 시작되고 온라인 편집 화면이 표시됩니다.



3. 파일을 편집할 수 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1388).png" alt=""><figcaption></figcaption></figure>
