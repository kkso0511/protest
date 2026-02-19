---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/security_doc_viewer
---

# 보안문서를 열람할 수 있는 사용자를 설정하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약한 경우, IRM(Information Rights Management)을 통해 의도치 않은 파일 유출을 방지할 수 있습니다.\
이 매뉴얼 에서는, [외부로 반출되는 파일의 보안을 설정하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/export_file_security)에서 설정된 작업 제한 범위 내에서 파일을 열람하거나 사용할 수 있는 SHIELD 사용자(IRM 사용 권한 사용자)를 추가하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* Guest, LDAP 연동 및 SAML 연동으로 추가된 사용자를 SHIELD 사용자로 설정할 수도 있습니다.
* Connect User는 SHIELD 사용자로 설정할 수 없습니다.
* DirectCloud-SHIELD IRM을 사용할 수 있는 상태라 하더라도, [특정 폴더에서 DirectCloud-SHIELD IRM을 활성화하는 방법](https://help.directcloud.net/admin_manual/folder/directcloud-shield-irm)에서 사용 여부를 사용하지 않음으로 설정한 경우에는 암호화가 적용되지 않습니다.

### 절차

1. 'SHIELD' > '사용자 선택' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

&#x20;      DirectCloud-SHIELD 사용자 설정 화면이 표시됩니다.

2. SHIELD 사용자로 활성화하여 설정하려는 사용자가 속한 그룹을 선택합니다.\
   Guest 사용자를 DirectCloud-SHIELD 사용자로 설정하려면 "Guest"를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

3. SHIELD 사용자로 활성화하여 설정하려는 사용자에 체크를 하고, 왼쪽 아래의 '사용개시' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (253).png" alt=""><figcaption></figcaption></figure>

4. 설정한 사용자의 상태가 '사용중'으로 변경되고, 상단 메뉴의 등록 사용자 수가 증가한 것을 확인합니다.

<figure><img src="../../.gitbook/assets/image (255).png" alt=""><figcaption></figcaption></figure>

5. DirectCloud-SHIELD 사용자를 비활성화하고 싶은 경우에는, 사용중인 사용자에 체크를 하고 왼쪽 아래의 '사용정지' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (256).png" alt=""><figcaption></figcaption></figure>

설정한 사용자의 상태가 미사용으로 변경됩니다.

<figure><img src="../../.gitbook/assets/image (257).png" alt=""><figcaption></figcaption></figure>
