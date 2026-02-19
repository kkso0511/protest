---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/folder/directcloud-shield-irm
---

# 특정 폴더에서 DirectCloud-SHIELD IRM을 활성화하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약하신 경우, IRM(Information Rights Management)을 이용하여 의도치 않은 파일 반출로 인한 정보 유출을 방지할 수 있습니다.\
이 매뉴얼에서는 관리자 페이지에서 폴더를 선택한 후, 폴더 속성에서 DirectCloud-SHIELD IRM을 활성화하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
*   DirectCloud-SHIELD IRM을 계약한 경우, [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)의 절차에서 DirectCloud-SHIELD IRM을 활성화하면 폴더 속성에 SHIELD가 표시됩니다.

    단, DirectCloud-SHIELD의 다른 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에는 폴더 속성에 SHIELD가 표시되지 않고, 관리자 페이지에DLP 관리 메뉴가 표시됩니다.
* 초기 상태에서는 SHIELD가 사용하지 않음으로 설정되어 있습니다.
* SHIELD는 Shared Box 메뉴의 1단계 폴더에만 설정할 수 있으며, 설정 내용은 하위 폴더로 자동으로 이어집니다.
* 업로드된 파일이 [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 지정한 파일 보안등급 판정 기준과 일치하는 경우, .irm 확장자가 추가됩니다.

<figure><img src="../../.gitbook/assets/image (2401).png" alt=""><figcaption></figcaption></figure>

* DirectCloud-SHIELD IRM에서는 확장자가 irm인 파일을 Storage 외부로 반출했을 때 암호화됩니다.
* 암호화된 파일을 DirectCloud-SHIELD IRM으로 열람할 수 있는 사용자를 설정하는 방법에서 DirectCloud-SHIELD IRM 사용 권한을 부여하면, Storage 외부로 반출된 파일에도 접근할 수 있습니다.
* DirectCloud-SHIELD IRM이 적용된 폴더에 업로드된 파일이 보안등급 판정 기준을 충족하는 경우, 파일이 업데이트되기 때문에 문서 관리 이하 폴더의 폴더 속성에서는 SHIELD 설정을 할 수 없습니다.
* DirectCloud-CONNECT를 이용할 수 있는 경우, 관리자 페이지에 Connect 관리 메뉴가 표시됩니다.
* Warm Storage를 이용할 수 있는경우, 관리자 페이지에 Warm Storage 관리 메뉴가 표시됩니다.
* Cold Storage를 계약한 경우, 관리자 페이지에 Cold Storage 관리 메뉴가 표시됩니다.

***

### 절차

1. '공유 설정' > 'Shared Box 관리'메뉴를 선택한 후, DirectCloud-SHIELD IRM을 활성화하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2402).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤한 후, 폴더 속성 설정에서 SHIELD의 '수정' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2403).png" alt=""><figcaption></figcaption></figure>



3. SHIELD 사용여부 설정에서 '사용'을 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2405).png" alt=""><figcaption></figcaption></figure>
