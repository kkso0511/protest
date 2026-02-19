---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/watermark_setting
---

# DLP 폴더에 저장된 파일에 표시되는 워터마크를 설정하는 방법

### 개요

DLP(Data Loss Prevention) 기능을 사용하면 사용자가 파일을 조작하거나 외부로 반출하는 행위를 제한할 수 있습니다. DLP 폴더에 기밀 정보가 포함된 파일을 저장하면 의도치 않은 파일 유출을 방지할 수 있습니다.이 매뉴얼 에서는 DLP 폴더에 저장된 파일에 ‘사외비’, ‘Confidential’ 등의 워터마크(투명 문자)를 설정하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* 워터마크 표시 설정은 기본으로 사용함으로 설정되어 있습니다.
* 워터마크는 아래 경우에 표시됩니다.
  * Web 브라우저: 미리보기
  * DirectCloud 드라이브: 미리보기, 직접 편집, 인쇄
*   워터마크 표시가 지원되는 확장자는 아래와 같습니다.&#x20;

    | 프로그램                 | 확장          |
    | -------------------- | ----------- |
    | Microsoft Excel      | xls、xlsx    |
    | Microsoft Word       | doc、docx    |
    | Microsoft PowerPoint | ppt、pptx    |
    | 기타                   | txt、pdf、dwg |

### 절차

{% hint style="warning" %}
**워터마크 표시 설정하기**
{% endhint %}

1. 'SHIELD' > 'DLP 설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>

2. 워터마크 설정에서 '사용'이 선택되어 있는지 확인한 뒤 상세설정 ▼ 을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

3. 워터마크 설정을 완료한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (185).png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="182.79998779296875">항목</th><th>설명</th></tr></thead><tbody><tr><td>적용범위</td><td><p>워터마크 표시가 적용될 작업에 체크합니다.</p><p>적용되는 작업은 아래와 같습니다.</p><ul><li>미리보기</li><li>문서열기(drive)</li><li>인쇄(drive)</li></ul></td></tr><tr><td>표시정보</td><td><p>워터마크에 표시할 정보에 체크합니다.<br>표시할 수 있는 정보는 다음과 같습니다.</p><ul><li><strong>사용자 ID</strong><br>파일을 미리보기 한 사용자의 ID</li><li><strong>시간</strong><br>파일을 미리보기 한 날짜와 시간</li><li><strong>추가 정보</strong><br>추가정보에 체크한 경우, 표시할 문자열을 100자 이내로 입력합니다.</li></ul></td></tr><tr><td>글자색상</td><td>▼ 버튼을 클릭하여 워터마크 텍스트의 색상을 선택합니다.</td></tr><tr><td>글자크기</td><td>슬라이드 버튼을 움직여 워터마크 텍스트의 크기를 설정합니다.<br>텍스트를 굵게 표시하려면 굵게에 체크합니다.</td></tr><tr><td>투명도</td><td>슬라이드 버튼을 움직여 워터마크의 투명도를 설정합니다.<br>투명도를 100%로 설정하면 워터마크가 표시되지 않게 됩니다.</td></tr><tr><td>표시 위치</td><td>워터마크의 표시 위치 정보가 표시됩니다.<br>표시 위치를 변경하려면 타일 버튼에서 변경할 영역을 선택합니다.</td></tr></tbody></table>

{% hint style="warning" %}
**워터마크 표시 예시**
{% endhint %}

아래에 워터마크 설정 예시와 표시 예시를 제공합니다.

* 워터마크 표시 설정 예시

<figure><img src="../../.gitbook/assets/image (185).png" alt="" width="563"><figcaption></figcaption></figure>

* 사용자 페이지에서 파일을 미리보기했을 때의 예시

<figure><img src="../../.gitbook/assets/image (186).png" alt=""><figcaption></figcaption></figure>
