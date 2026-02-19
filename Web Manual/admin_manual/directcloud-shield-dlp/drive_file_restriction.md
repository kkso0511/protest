---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/drive_file_restriction
---

# DirectCloud 드라이브의 DLP 폴더에 저장된 파일의 작업을 제한하는 방법

### 개요

DLP(Data Loss Prevention) 기능을 사용하면 사용자가 파일을 조작하거나 외부로 반출하는 행위를 제한할 수 있습니다. DLP 폴더에 기밀 정보가 포함된 파일을 저장하면 의도치 않은 파일 유출을 방지할 수 있습니다.이 매뉴얼 에서는 DirectCloud 드라이브의 DLP 폴더에 저장된 파일의 작업을 제한하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* 제한할 수 있는 작업은 아래와 같습니다.
  * 스크린샷
  * 텍스트 복사
  * 인쇄
* 화면 캡처 및 텍스트 복사 금지 기능에서 사용함을 선택한 경우 스크린샷 촬영이 제한되는 애플리케이션은 Windows 기본 제공 도구인 '캡처도구'만 해당합니다.
* DirectCloud 드라이브의 DLP 폴더에서는 아래 애플리케이션에서 파일을 열 수 있습니다.\
  또한 아래 애플리케이션에서는 화면 캡처 및 텍스트 복사 금지 기능에서 사용함을 선택했을 때 텍스트 복사가 제한되며, 인쇄 금지 기능에서 사용함을 선택했을 때 인쇄가 제한됩니다.
  * Microsoft Notepad
  * Microsoft Excel
  * Microsoft Word
  * Microsoft PowerPoint
  * Adobe Acrobat
  * Adobe Reader
  * Autodesk AutoCAD
* 스크린샷 또는 텍스트 복사 중 하나만 개별적으로 제한하는 것은 불가능합니다.
* Web 브라우저에서 파일을 온라인 편집할 때의 작업 제한 내용은 [파일을 다운로드 하지 않고 온라인으로 편집할 수 있도록 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/online_edit)에 따라 달라집니다.
* 덮어쓰기 저장 및 다른 이름으로 저장 작업은 제한할 수 없습니다.
* DLP 설정 메뉴는 DirectCloud의 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에 표시됩니다.
* DirectCloud-SHIELD DLP는 다른 유료 옵션인 DirectCloud-SHIELD IRM으로 전환할 수 있습니다. \
  자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.

### 절차

{% hint style="warning" %}
**작업 제한 설정하기**
{% endhint %}

1. 'SHIELD' > 'DLP 설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>

2. 'DRIVE 편집 제어' 설정 항목에서 아래 내용을 설정한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (181).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="219.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>화면캡쳐 및 복사 방지</td><td>'사용'을 선택하면 스크린샷 및 텍스트 복사가 제한됩니다.</td></tr><tr><td>인쇄방지</td><td>'사용'을 선택하면 인쇄가 제한됩니다.</td></tr></tbody></table>

{% hint style="warning" %}
**제한된 작업을 수행한 경우**
{% endhint %}

DirectCloud 드라이브에서 DirectCloud 드라이브에서의 작업 제한 설정에 의해 제한된 작업을 수행하면 화면 오른쪽 아래에 아래 메시지가 표시됩니다.

* 스크린샷\
  '보안 모드가 동작중입니다. 화면캡처 방지가 실행되었습니다.'
* 텍스트 복사\
  '보안 모드가 동작중입니다. 복사방지가 실행되었습니다.'
* 인쇄\
  '보안 모드가 동작중입니다. 인쇄방지가 실행되었습니다.'
