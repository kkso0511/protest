---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/check_capacity
---

# DLP 관리 메뉴에서 계약 용량을 확인하는 방법

### 개요

DLP(Data Loss Prevention) 기능을 사용하면 사용자가 파일을 조작하거나 외부로 반출하는 행위를 제한할 수 있습니다. DLP 폴더에 기밀 정보가 포함된 파일을 저장하면 의도치 않은 파일 유출을 방지할 수 있습니다.이 매뉴얼 에서는 '공유 설정' > 'DLP 관리' 메뉴에서 DLP의 계약 용량을 확인하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목에 접근할 수 있습니다.
* DLP 폴더와 DLP 관리 메뉴는 DirectCloud의 유료 옵션인 DirectCloud-SHIELD DLP를 계약한 경우에만 표시됩니다.
* Shared Box와는 달리, DLP 관리 메뉴에서는 대상 사용자가 모든 사용자의 폴더를 생성할 수 없습니다.
* DLP 관리의 폴더 속성에는 다음 설정 항목이 표시됩니다:
  * PDF 다운로드 설정
  * 다운로드 설정
  * 링크 설정
  * 파일첨부 메일발송 설정
* DLP 관리 메뉴에서는 접근 권한 추가 알림 메일 설정을 할 수 없습니다.
* DLP 폴더의 폴더 속성에서는 워크플로우, SHIELD, 링크를 설정할 수 없습니다.
* DLP 폴더에서는 Connect User 초대를 할 수 없습니다.
* 폴더 속성의 용량 제한 설정에서는 DLP의 계약 용량을 초과하는 용량을 할당할 수 없습니다.
*   DLP 폴더는 Shared Box와 마찬가지로 노드값이라는 고유한 값으로 관리됩니다. 이 값은 DirectCloud 관리자 API에서 폴더를 지정할 때 사용됩니다.\
    루트 폴더에는 1{8이라는 값이 할당되어 있으며, 하위 계층에 폴더가 생성될 때마다 3자씩 노드값이 추가됩니다.\
    예시는 다음과 같습니다:

    * 제1계층: 1{8Sh8
    * 제2계층: 1{8Sh89ZT
    * 제3계층: 1{8Sh89ZT9jK

    일괄 등록에서는 이미 동일한 이름(노드값)의 폴더가 있는 경우 스킵 처리됩니다.

### 절차

1. '공유 설정' > 'DLP 관리' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2471).png" alt=""><figcaption></figcaption></figure>

2. 계약용량에 표시된 용량을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2472).png" alt=""><figcaption></figcaption></figure>
