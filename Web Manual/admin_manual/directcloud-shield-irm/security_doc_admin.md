---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/security_doc_admin
---

# 보안문서 해제나 보안등급을 변경할 수 있는 ‘보안문서 관리자’를 설정하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약하고 있는 경우, IRM(Information Rights Management)을 이용하여 의도하지 않은 파일의 유출을 방지할 수 있습니다.\
이 매뉴얼 에서는, DirectCloud-SHIELD IRM으로 암호화된 파일의 암호화를 해제하거나 보안등급을 변경할 수 있는 보안문서 관리자에 사용자를 추가하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* LDAP 연동 및 SAML 연동으로 추가된 사용자도 보안문서 관리자로 설정할 수 있습니다.
* Guest와 Connect User는 보안문서 관리자로 설정할 수 없습니다.
*   보안문서 관리자 설정에서는 기본적으로 '시스템 관리자 모두 포함'과 'Shared Box의 각 폴더마스터 모두 포함'에 체크되어 있기 때문에, 계약 담당 관리자, 일반 관리자, '마스터'에게는 보안문서 관리자 권한이 부여되어 있습니다.

    또한 Shared Box, Connect, DLP, Warm Storage 메뉴 중 어느 하나의 폴더라도 '마스터' 권한이 부여된 사용자는, 보안문서 관리자로서 해당 모든 폴더에서 파일의 암호화를 해제할 수 있습니다.
* [보안문서 설정을 관리자 페이지에서 해제하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/release_security_doc) 또는 [사용자 페이지에서 파일의 보안문서 설정을 해제하는 방법](https://help.directcloud.net/user_manual/file_management/irm_unlock)으로 암호화를 해제하면, 보안등급 라벨이 표시되지 않게 됩니다.
* [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/security_criteria)에서 상태를 비활성으로 설정하면, 보안등급 라벨이 보안등급 없음으로 변경됩니다.

### 절차

{% hint style="warning" %}
**보안문서 관리자를 설정하기**
{% endhint %}

1. 'SHIELD' > '사용자 선택' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2385).png" alt=""><figcaption></figcaption></figure>

2. 화면을 아래로 스크롤한 뒤, 보안문서 관리자 설정의 사용자 추가 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2386).png" alt=""><figcaption></figcaption></figure>

3. 보안문서 관리자로 추가하려는 사용자의 이름 또는 ID를 입력하고, 검색 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2387).png" alt=""><figcaption></figcaption></figure>

4. 검색 결과에 표시된 사용자의 추가 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2388).png" alt=""><figcaption></figcaption></figure>

5. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2389).png" alt=""><figcaption></figcaption></figure>
