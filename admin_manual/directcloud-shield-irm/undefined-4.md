---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/undefined-4
---

# 외부로 반출되는 파일의 보안을 설정하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약하고 있는 경우, IRM(Information Rights Management)을 사용하여 의도하지 않은 파일 유출을 방지할 수 있습니다.\
이 매뉴얼에서는, [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 설정한 문서 속성에 따라 외부로 반출된 파일의 보안 설정(사용 가능한 사용자, 유효 기간, 개봉 횟수 등)을 지정하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* 반출 문서 보안 설정을 표시하려면, '반입 문서 보안'의 저장 방법을 '라벨 표시 후 암호화'로 선택해야 합니다.
* 화면 및 텍스트 복사 금지에서 사용을 선택한 경우, 스크린샷 촬영이 제한되는 애플리케이션은 Windows 기본 프로그램인 <캡쳐도구>만 해당됩니다.
* 반출 문서 보안의 암호화 설정에서 '화면 캡쳐 방지 및 복사 금지'가 선택되어 있지 않더라도, 암호화된 파일은 다른 이름으로 저장 기능을 통해 저장할 수 없습니다.
*   DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)에서는 다음 애플리케이션에서 파일을 열 수 있습니다.\
    또한 아래 애플리케이션에서는 문서의 반출 시 보안 설정의 암호화 설정에서 화면 및 텍스트 복사 금지에 체크했을 때 텍스트 복사와 덮어쓰기 저장이 제한되며, 인쇄 금지에 체크했을 때 인쇄가 제한됩니다.

    Microsoft Notepad\
    Microsoft Excel\
    Microsoft Word\
    Microsoft PowerPoint\
    Adobe Acrobat\
    Adobe Reader\
    Autodesk AutoCAD 2023, 2024, 2025
* DirectCloud-SHIELD IRM에서는 외부로 반출되는 문서를 32자리 고유 식별 번호로 관리합니다.
* 유효 기간 제한과 개봉 횟수 제한 설정은 식별 번호마다 적용됩니다.\
  다만, DirectCloud 드라이브에서는 파일을 열 때마다 서로 다른 식별 번호가 부여되어 횟수가 리셋되기 때문에, 유효 기간 제한과 개봉 횟수 제한 설정은 적용되지 않습니다.
* DirectCloud-SHIELD IRM을 사용할 수 있는 상태라 하더라도, [특정 폴더에서 DirectCloud-SHIELD IRM을 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-4/directcloud-shield-irm)에서 사용 여부를 사용하지 않음으로 설정한 경우에는 암호화가 적용되지 않습니다.

### 절차

{% hint style="info" %}
**보안수준 정의 화면을 표시하기**
{% endhint %}

1. 'SHIELD' > '설정' 메뉴를 선택하고 '보안수준 정의' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (246).png" alt=""><figcaption></figcaption></figure>

2. 동작 열에 표시된 버튼을 클릭합니다.\
   업로드 대상 파일이, [보안 문서 판단 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 지정한 문서 속성 중 어느 항목에 해당하는지 확인한 뒤, 그에 맞는 보안수준을 선택합니다.

<figure><img src="../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

&#x20;      선택한 보안수준의 보안수준 정의 화면이 표시됩니다.

{% hint style="info" %}
**반출 파일의 작업 제한을 설정하기**
{% endhint %}

**반출 문서 보안을 설정하기**

1. '보안수준 정의' > '반출 문서 보안'에서 아래 항목을 설정한 후 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (248).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="147.5999755859375">항목</th><th>내용</th></tr></thead><tbody><tr><td>사용범위</td><td><p>암호화된 파일에 대한 작업 제한으로 아래 중 하나를 선택합니다.<br></p><ul><li><strong>전 기능 사용</strong><br>파일에 대해 작업 제한을 하지 않을 경우 선택합니다.</li><li><p><strong>읽기만 가능</strong><br>파일에 대해 작업 제한을 적용할 경우 선택합니다.<br>금지할 작업으로는 아래 두 가지 중에서 선택할 수 있습니다.</p><ul><li>화면 캡처 방지 및 복사 방지<br>스크린샷, 텍스트 복사, 덮어쓰기 저장을 금지할 경우 선택합니다.</li><li>인쇄 방<br>인쇄를 금지할 경우 선택합니다.</li></ul></li></ul></td></tr><tr><td>유효기간 제한</td><td>반출한 파일을 표시할 수 있는 기간을 설정합니다.<br>사용을 선택하고, 1~365 범위에서 일수를 입력합니다.</td></tr><tr><td>열람횟수 제한</td><td>반출한 파일을 표시할 수 있는 횟수를 설정합니다.<br>사용을 선택하고, 1~99 범위에서 횟수를 입력합니다.</td></tr></tbody></table>



**반출 문서 보안의 설정 값에 대해**

인증 후 DirectCloud-SHIELD IRM에 로그인하면, 사용 권한에서 '반출 문서 보안' 항목의 설정 값을 확인할 수 있습니다.

* 관리자 페이지의 반출 문서 보안 설정

<figure><img src="../../.gitbook/assets/image (248).png" alt=""><figcaption></figcaption></figure>

* DirectCloud-SHIELD IRM의 사용 권한

<figure><img src="../../.gitbook/assets/image (2406).png" alt="" width="370"><figcaption></figcaption></figure>

{% hint style="info" %}
**반출 파일에 워터마크를 표시하기**
{% endhint %}

**반출 파일의 워터마크를 설정하기**

1. '보안수준 정의'의 '반출 문서 보안'에서 워터마크의 사용을 선택하고, '상세설정▼'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (249).png" alt=""><figcaption></figcaption></figure>

2. 워터마크를 설정한 후 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (250).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="182.79998779296875">항목</th><th>설명</th></tr></thead><tbody><tr><td>적용범위</td><td><p>아래 항목에 체크하면, 해당되는 경우 워터마크가 표시됩니다.<br></p><ul><li><strong>문서열기</strong><br>파일을 미리보기 했을 때 워터마크를 표시합니다.</li><li><strong>인쇄</strong><br>파일을 인쇄했을 때 용지에 워터마크를 표시합니다.</li></ul></td></tr><tr><td>표시정보</td><td><p>워터마크에 표시할 정보에 체크합니다.<br>표시할 수 있는 정보는 다음과 같습니다.<br></p><ul><li><strong>사용자 ID</strong><br>파일을 미리보기 한 사용자의 ID</li><li><strong>시간</strong><br>파일을 미리보기 한 날짜와 시간</li><li><strong>보안등급</strong><br>보안수준 정의에 표시되어 있는 보안등급</li><li><strong>추가 정보</strong><br>추가정보에 체크한 경우, 표시할 문자열을 100자 이내로 입력합니다.</li></ul></td></tr><tr><td>글자색상</td><td>▼ 버튼을 클릭하여 워터마크 텍스트의 색상을 선택합니다.</td></tr><tr><td>글자크기</td><td>슬라이드 버튼을 움직여 워터마크 텍스트의 크기를 설정합니다.<br>텍스트를 굵게 표시하려면 굵게에 체크합니다.</td></tr><tr><td>투명도</td><td>슬라이드 버튼을 움직여 워터마크의 투명도를 설정합니다.<br>투명도를 100%로 설정하면 워터마크가 표시되지 않게 됩니다.</td></tr><tr><td>표시 위치</td><td><p>워터마크의 표시 위치 정보가 표시됩니다.<br></p><ul><li>센터사선 표시<br>파일 중앙에 하나의 워터마크가 사선으로 표시됩니다.</li><li>바둑판식 채우기(사선 표시)<br>PC 전체 화면에 여러 개의 워터마크가 사선으로 반복 표시됩니다.</li><li>바둑판식 채우기(수평 표시)<br>PC 전체 화면에 여러 개의 워터마크가 수평으로 반복 표시됩니다.</li><li>위치지정(수평 표시)<br>워터마크를 표시할 영역의 타일 버튼을 클릭하면, PC 화면의 해당 영역에 하나의 워터마크가 수평으로 표시됩니다.</li></ul></td></tr></tbody></table>



**워터마크 표시 예**

아래에서는 워터마크 설정 예와 표시 예를 보여드립니다.

* 워터마크의 설정 예

<figure><img src="../../.gitbook/assets/image (250).png" alt=""><figcaption></figcaption></figure>

* 반출 파일의 워터마크 표시 예

<figure><img src="../../.gitbook/assets/image (2407).png" alt=""><figcaption></figcaption></figure>

