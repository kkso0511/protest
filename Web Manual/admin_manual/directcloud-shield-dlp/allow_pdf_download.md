---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/allow_pdf_download
---

# 'DLP 설정'에서 사용자에게 파일을 PDF로 다운로드할 수 있는 기능을 허용하는 방법

### 개요

DLP(Data Loss Prevention) 기능을 사용하면 사용자가 파일을 조작하거나 외부로 반출하는 행위를 제한할 수 있습니다. DLP 폴더에 기밀 정보가 포함된 파일을 저장하면 의도치 않은 파일 유출을 방지할 수 있습니다.이 매뉴얼 에서는 'SHIELD' > 'DLP 설정' 메뉴에서 Web 브라우저 및 DirectCloud 드라이브의 DLP 폴더에 저장된 파일을 PDF로 변환하여 다운로드할 수 있도록 설정하는 방법을 설명합니다.\
또한 다운로드되는 PDF 파일에 ‘사외비’, ‘Confidential’ 등의 워터마크(투명 문자)를 적용하는 방법도 함께 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* PDF 다운로드 설정은 기본으로 사용으로 설정되어 있습니다.
* PDF를 다운로드하려는 사용자에게는 다음의 접근 권한이 부여되어 있어야 합니다.\
  <마스터>,<전체권한>,<편집자>,<다운로더>
*   PDF 다운로드가 지원되는 확장자는 아래와 같습니다.

    | 프로그램                 | 확장       |
    | -------------------- | -------- |
    | Microsoft Excel      | xls、xlsx |
    | Microsoft Word       | doc、docx |
    | Microsoft PowerPoint | ppt、pptx |
    | 기타                   | pdf、dwg  |
* 아래 설정과 다르게, '워크플로우' > '설정' 메뉴의 워크플로우 기본 설정에서 DLP 다운로드 워크플로우가 활성화되어 있지 않더라도 PDF 다운로드 설정은 가능합니다.
  * 다운로드 설정
  * 링크 설정
  * 첨부 파일 전송 설정
* DLP 설정 메뉴는 DirectCloud의 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에 표시됩니다.
* DirectCloud-SHIELD DLP는 다른 유료 옵션인 DirectCloud-SHIELD IRM으로 전환할 수 있습니다. \
  자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.

### 절차

{% hint style="warning" %}
**워터마크를 추가하지 않는 경우**
{% endhint %}

1. 'SHIELD' > 'DLP 설정' 메뉴를 선택하고 '파일 반출 정책' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

2. PDF 다운로드 설정에서 '사용'이 선택되어 있는지 확인한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**워터마크를 추가하는 경우**
{% endhint %}

1. 'SHIELD' > 'DLP 설정' 메뉴를 선택하고 '파일 반출 정책' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

2. PDF 다운로드 설정에서 '사용'을 선택하고, 워터마크 항목에 체크한 뒤 상세설정 ▼ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

3. 워터마크 설정을 진행합니다.

<figure><img src="../../.gitbook/assets/image (179).png" alt="" width="549"><figcaption></figcaption></figure>

<table><thead><tr><th width="182.79998779296875">항목</th><th>설명</th></tr></thead><tbody><tr><td>표시정보</td><td><p>워터마크에 표시할 정보에 체크합니다.<br>표시할 수 있는 정보는 다음과 같습니다.</p><ul><li><strong>사용자 ID</strong><br>파일을 미리보기 한 사용자의 ID</li><li><strong>시간</strong><br>파일을 미리보기 한 날짜와 시간</li><li><strong>추가 정보</strong><br>추가정보에 체크한 경우, 표시할 문자열을 100자 이내로 입력합니다.</li></ul></td></tr><tr><td>글자색상</td><td>▼ 버튼을 클릭하여 워터마크 텍스트의 색상을 선택합니다.</td></tr><tr><td>글자크기</td><td>슬라이드 버튼을 움직여 워터마크 텍스트의 크기를 설정합니다.<br>텍스트를 굵게 표시하려면 굵게에 체크합니다.</td></tr><tr><td>투명도</td><td>슬라이드 버튼을 움직여 워터마크의 투명도를 설정합니다.<br>투명도를 100%로 설정하면 워터마크가 표시되지 않게 됩니다.</td></tr><tr><td>표시 위치</td><td>워터마크의 표시 위치 정보가 표시됩니다.<br>표시 위치는 '센터 사선 표시'로고정됩니다.</td></tr></tbody></table>

4. '저장' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (180).png" alt="" width="549"><figcaption></figcaption></figure>

{% hint style="warning" %}
**워터마크 표시 예시**
{% endhint %}

아래에 워터마크 설정 예시와 PDF 표시 예시를 제공합니다.

* 'PDF 다운로드' 설정 예시

<figure><img src="../../.gitbook/assets/image (179).png" alt="" width="549"><figcaption></figcaption></figure>

* 다운로드한 PDF 파일의 예시

<figure><img src="../../.gitbook/assets/image (2449).png" alt=""><figcaption></figcaption></figure>

