---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_management/d_irm
---

# \[Drive] DirectCloud-SHIELD IRM 통합 버전에서 암호화된 파일을 이용하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약하신 경우, IRM(Information Rights Management)을 이용하여 의도치 않은 파일 유출을 방지할 수 있습니다.\
DirectCloud-SHIELD IRM 기능이 활성화된 폴더에서는, 관리자의 설정에 따라 파일이 암호화됩니다.\
이 매뉴얼 에서는 DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)를 사용하여 DirectCloud-SHIELD IRM으로 암호화된 파일을 표시하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 본 매뉴얼의 절차를 실행하려면 DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)가 설치되어 있어야 합니다.
* DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)는 Windows용 64bit 애플리케이션만 제공됩니다.\
  Mac용 애플리케이션은 제공되지 않습니다.
* DirectCloud-SHIELD IRM으로 암호화된 파일은 Windows의 Microsoft Office 애플리케이션에서 직접 열람할 수 없습니다.\
  아래 방법 중 하나로 표시해야 합니다.
  * 다음 중 하나를 설치하고 파일을 더블 클릭하여 표시\
    • DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)(본 매뉴얼 절차)\
    • DirectCloud-SHIELD IRM PC 전용 애플리케이션
  * DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)를 설치한 뒤, 파일 미리보기 또는 편집을 선택하여 표시합니다.
* [사용자가 이용할 수 있는 애플리케이션을 제한하는 방법](https://help.directcloud.net/admin_manual/security_policy/app_restrictions)에서 DirectCloud 드라이브가 허용되어 있지 않으면 DirectCloud 드라이브에 로그인할 수 없습니다.
* DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)에서는 일반 DirectCloud 드라이브와 동일한 작업을 수행할 수 있습니다.\
  자세한 내용은 [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/d_permission)을 참고해주시기 바랍니다.
* 본 매뉴얼의 절차는 DirectCloud-SHIELD IRM PC 전용 애플리케이션에서 파일을 표시할 때와 달리, 로그인 화면이 표시되지 않습니다.\
  따라서 SHIELD 사용자 또는 2단계 인증 사용자로 로그인하기 위한 설정을 할 수 없으므로, 관리자 페이지의 DirectCloud-SHIELD 사용자 설정에서 상태가 미사용으로 되어 있는 사용자 또는 2단계 인증 사용자가 irm 확장자 파일을 열려고 하면 파일을 열 권한이 없습니다라고 표시됩니다.
* DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)에서는 다음 애플리케이션에서 파일을 열 수 있습니다.\
  또한 다음 애플리케이션에서는 문서 반출 시 보안 설정의 암호화 설정에서 화면 및 텍스트 복사 금지에 체크한 경우 텍스트 복사와 덮어쓰기 저장이 제한되며, 인쇄 금지에 체크한 경우 인쇄가 제한됩니다.&#x20;
  * Microsoft 메모장
  * Microsoft Excel
  * Microsoft Word
  * Microsoft PowerPoint
  * Adobe Acrobat
  * Adobe Reader
  * Autodesk AutoCAD 2023, 2024, 2025

### 절차

1.  DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)에서 DirectCloud 폴더를 표시합니다.

    확장자가 irm인 파일을 더블 클릭합니다.

<figure><img src="../../.gitbook/assets/image (213).png" alt=""><figcaption></figcaption></figure>

2. DirectCloud-SHIELD 화면이 표시됩니다. \
   동의함에 체크한 뒤 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (214).png" alt=""><figcaption></figcaption></figure>

3. 파일 형식에 대응하는 애플리케이션에서 파일이 표시됩니다.\
   [외부로 반출되는 파일의 보안을 설정하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-4) 설정에 따라 워터마크(투명 문자)가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>
