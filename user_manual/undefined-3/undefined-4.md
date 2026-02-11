---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-3/undefined-4
---

# 사용자 페이지에서 파일의 보안등급을 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약하신 경우, IRM(Information Rights Management)을 이용하여 의도치 않은 파일 반출로 인한 정보 유출을 방지할 수 있습니다.\
DirectCloud-SHIELD IRM 기능이 활성화된 폴더에서는, 관리자의 설정에 따라 파일에 보안등급 라벨이 표시되고 .irm 확장자가 추가됩니다.\
이 매뉴얼 에서는 사용자 페이지에서 DirectCloud-SHIELD IRM에 의해 부여된 파일의 보안등급 라벨을 변경하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 파일의 보안등급 라벨은 DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약한 경우에만 표시됩니다.\
  또한 파일의 보안등급 라벨은 Web 브라우저에서만 표시됩니다.
* DirectCloud-SHIELD IRM이 활성화된 폴더에 보안 문서 판정 기준에 해당하는 파일이 포함된 폴더를 업로드하면, [업로드한 파일을 판정 기준에 따라 보안하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-3)에 따라 업로드된 파일에 자동으로 보안등급 라벨이 적용됩니다.\
  또한 파일이 Storage 외부로 반출될 경우 암호화가 적용됩니다.
* 파일의 보안등급 라벨을 변경해도 버전은 업데이트되지 않습니다.
* 관리자가 [파일의 보안등급을 변경하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-7)을 통해 보안등급을 수정할 수도 있습니다.
* 본 매뉴얼 및 [파일의 보안등급을 변경하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-7)에서는 모든 보안등급 라벨을 제거하여 보안등급 없음으로 설정할 수 없습니다.
* [보안문서 설정을 관리자 페이지에서 해제하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-8) 또는 사용자 페이지에서 해제하는 방법을 통해 관리자가 설정한 보안수준 정의를 해제하면 보안등급 라벨이 제거되고 .irm 확장자가 표시되지 않게 됩니다.

### 절차

1. 파일의 보안등급 라벨을 클릭합니다.\
   보안문서 정의 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2411).png" alt=""><figcaption></figcaption></figure>

2. 편집 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2413).png" alt="" width="563"><figcaption></figcaption></figure>

3. 문서 속성에서 파일에 설정할 보안등급을 클릭하여 선택한 뒤 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2415).png" alt="" width="563"><figcaption></figcaption></figure>

4. 확인 버튼을 클릭합니다.\
   암호화 해제 버튼을 클릭하면 Storage 외부로 반출될 때 적용되는 암호화 설정을 해제하고 보안등급 라벨을 제거할 수 있습니다.\
   단, 보안등급 라벨은 원래 상태로 되돌릴 수 없으므로 주의가 필요합니다.

<figure><img src="../../.gitbook/assets/image (2416).png" alt=""><figcaption></figcaption></figure>
