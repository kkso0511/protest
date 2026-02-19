---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_management/wd_download
---

# \[Web, Drive] 파일을 다운로드하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 파일을 다운로드하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 Shared Box에서 작업하는 방법에 대해 설명하지만 Shared Box 이외의 폴더에 대해서도 비슷한 절차를 수행할 수 있습니다.
* 파일을 다운로드하는 사용자에게는 <마스터>, <전체권한>, <편집자>, <다운로더>에 대한 접근권한이 부여되어야 합니다.
* Google 크롬, Microsoft Edge 및 Mozilla Firefox에서 여러 파일을 다운로드하는 경우 최대 5개의 파일을 개별적으로 다운로드합니다.\
  폴더 또는 6개 이상의 파일을 선택하여 다운로드하면 ZIP 형식의 파일로 압축됩니다.\
  Safari에서 여러 파일을 다운로드하는 경우 파일 수에 관계없이 ZIP 형식의 파일로 압축됩니다.
* ZIP 형식으로 압축된 파일의 용량이 2GB를 초과하면 DirectCloud에서 다운로드할 수 없습니다.
* DirectCloud에 저장된 ZIP 파일을 다운로드할 때 용량 한도는 없습니다.
* ZIP 형식의 파일로 일괄 다운로드 한 후, 압축을 푼 파일이 깨져 버린 경우는, 7-Zip 등의 UTF-8 인코딩에 대응하고 있는 압축 압축 해제 소프트웨어나, Windows 익스플로러의 서고 압축 해제 기능을 이용해 해동해 주세요.
* Lhaplus와 같은 UTF-8 인코딩을 지원하지 않는 압축 해제 소프트웨어로 파일을 압축 해제하면 깨질 수 있습니다.
* Web 브라우저에서는 드래그 앤 드롭으로 파일을 다운로드할 수 없습니다.\
  PC Agent 또는 DirectCloud 드라이브를 사용하십시오.
* Shared Box, Connect, DLP, Warm Storage, Cold Storage의 첫 번째 계층 폴더를 모두 선택하여 폴더와 파일을 일괄 다운로드할 수는 없습니다.
* 다운로드가 완료되면 알림 이메일이 전송되지 않습니다.
* 워크플로우가 활성화 된 경우, ‘결재선 미지정사용자’ 설정에서 ‘기능을 제한함’이 선택된 경우, 워크플로 신청자로 설정된 사용자가 아닌 경우에는 파일을 다운로드할 수 없습니다.
* [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)에서 워크플로우에 포함되지 않은 사용자 설정의 기능을 제한하기가 선택된 경우, 워크플로우 신청자로 설정된 사용자 이외에는 파일을 다운로드할 수 없습니다.
* [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)에서 기본 설정 화면의 다운로드 항목에 체크되어 있는 경우, '보안정책' > '모바일 보안'메뉴의 메일 전송, 다른 앱으로 열기 설정이 사용하지 않음으로 고정되며, 모바일 애플리케이션에 다운로드와 이미지 저장 기능이 표시되지 않습니다.\
  자세한 내용은 [모바일 메뉴의 각 설정 항목이 '사용 안 함'으로 고정된 경우 해결 방법](https://help.directcloud.net/admin_manual/security_policy/m_menu_activation)을 참고해주시기 바랍니다.
* 워크플로우가 비활성화된 상태에서 DirectCloud에 파일을 남기지 않고 다운로드하려면 '마스터', '전체권한', '편집자' 접근 권한이 필요합니다.
* DirectCloud-CONNECT를 사용할 수 있는 경우, 사용자 페이지에 Connect 메뉴가 표시됩니다.
* DirectCloud-SHIELD DLP를 계약한 경우, 사용자 페이지에 DLP 메뉴가 표시되고 DirectCloud 드라이브에 DLP 폴더가 표시됩니다.
* DLP 폴더의 파일을 다운로드하려면, DLP 설정에서 사용자에게 다운로드를 허용하도록 설정하는 절차에서 다운로드 설정을 사용함으로 지정해야 합니다.
* Warm Storage를 기본으로 사용할 수 있는경우, 사용자 페이지에 Warm Storage 메뉴가 표시되고 DirectCloud 드라이브에 Warm Storage 폴더가 표시됩니다.
* Cold Storage를 계약한 경우, 사용자 페이지에 Cold Storage 메뉴가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 파일 다운로드**
{% endhint %}

1. 다운로드할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1418).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나로 파일을 다운로드합니다.

❶  다운로드하고자 하는 파일을 체크하고 상단의 '다운로드' 버튼을 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1419).png" alt=""><figcaption></figcaption></figure>

❷  다운로드하고자 하는 파일을 체크하고 우클릭하여 표시된 메뉴에서 '다운로드'를 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1420).png" alt=""><figcaption></figcaption></figure>

❸  다운로드할 파일의 오른쪽에 있는 ▼ 버튼을 클릭한 후 표시된 메뉴에서 '다운로드'를 클릭합니다. 여러 파일을 선택할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (1421).png" alt=""><figcaption></figcaption></figure>



3. 다운로드한 파일을 확인합니다.

<figure><img src="../../.gitbook/assets/image (1422).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 파일 다운로드**
{% endhint %}

**\[다운로드할 파일 보기]**

1. 다운로드할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1423).png" alt=""><figcaption></figcaption></figure>



**\[워크플로우가 비활성화된 상태에서 파일 다운로드]**

워크플로우가 사용 안 함으로 설정된 경우 드래그 앤 드롭으로 파일을 다운로드할 수 있습니다.

1. DirectCloud에 파일을 남긴 상태로 다운로드하려면 파일을 드래그하여 PC의 폴더나 바탕 화면에 놓습니다.

<figure><img src="../../.gitbook/assets/image (1425).png" alt=""><figcaption></figcaption></figure>

파일이 복사됩니다.



2. DirectCloud에 파일을 남기지 않고 다운로드하려면 "Shift" 키를 누른 상태에서 PC의 폴더 또는 바탕 화면으로 파일을 끌어다 놓습니다.



**\[워크플로우가 활성화된 상태에서 파일 다운로드]**

워크플로우를 사용하도록 설정한 경우 오른쪽 클릭으로 표시되는 컨텍스트 메뉴에서 파일 다운로드를 신청할 수 있습니다.

1. 다운로드할 파일을 마우스 오른쪽 버튼으로 클릭하고 표시되는 메뉴에서 DirectCloud 드라이브 > 다운로드를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1426).png" alt=""><figcaption></figcaption></figure>

다운로드 워크플로우 화면이 표시됩니다.



2. 워크플로우를 설정하고 신청 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1427).png" alt=""><figcaption></figcaption></figure>

신청이 승인되면 파일이 다운로드됩니다.
