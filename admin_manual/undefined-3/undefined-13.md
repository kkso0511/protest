---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-3/undefined-13
---

# 사용자 정보 일괄 추가로 깨진 경우의 해결 방법 (일본어 문제로 한국불필요)

### 개요 <a href="#a03" id="a03"></a>

사용자 정보를 일괄로 추가하는 방법으로 사용자를 일괄 추가하면 이자체 등이 포함된 이름이 깨져 등록될 수 있습니다.\
이 절에서는 사용자 일괄 처리에서 사용한 CSV 파일로 인해 깨진 상태로 등록되어 버리는 경우의 해결 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 [관리자의 기능 제한](https://boxmanager.directcloud.jp/setting/manager) 으로 "사용자"를 선택해야 합니다.
* Microsoft Office 2013 이전 버전은 유니코드를 지원하지 않으므로 해당 버전을 사용하는 경우 내보낼 파일의 문자 코드로 Shift\_JIS를 선택해야 합니다.
* 사용자 일괄 처리 화면에서 내보내는 사용자 정보, 템플릿, 그룹 코드 CSV 파일의 문자 코드는 환경 설정 > 고급 설정 메뉴의 CSV 내보내기시 문자 코드 설정에서 설정됩니다. .\
  자세한 내용은 [내보낼 CSV 파일의 문자 코드를 설정하는 방법을](https://help.directcloud.jp/s/article/operation-of-administrator-function11267) 참조하십시오.

### 절차 <a href="#a05" id="a05"></a>

사용자 목록 페이지는 문자 코드가 UTF-8로 고정되어 있으므로 UTF-8의 한자, 히라가나, 영대 소문자, 숫자, 공백, 다국어 문자, 기호 및 이모티콘 등에 해당합니다.\
그러나 문자 코드가 Shift\_JIS의 CSV 파일로 내보내면 이자체와 같은 일부 문자가 깨질 수 있습니다.\
또한 내보낸 템플릿을 사용하여 가져오기용 CSV 파일을 만들 때 문자 코드를 Shift\_JIS로 저장하면 이문자 등이 깨진 상태로 저장될 수 있습니다. 해당 CSV 파일을 가져오면 깨진 상태로 사용자가 등록됩니다.\
이 문제를 해결하려면 다음 단계를 따르십시오.

1. [내보낼 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11267) 으로 내보낼 파일의 문자 코드를 "UTF-8 BOM 포함"으로 설정합니다.
2. 사용자 > 사용자 관리 메뉴를 선택하고 사용자 일괄 처리 버튼을 클릭하여 CSV 파일을 내보냅니다.
3. [사용자를 대량으로 추가하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11088) 과 [사용자 정보를 대량으로 변경하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11089)  의 단계에서 2단계에서 다운로드한 CSV 파일에 필요한 정보를 제공합니다.
4. 3단계에서 편집한 CSV 파일을 가져옵니다.
