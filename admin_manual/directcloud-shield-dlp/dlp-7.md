---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-dlp/dlp-7
---

# DLP 폴더 속성에서 파일첨부 메일발송을 활성화하는 방법

### 개요

이 매뉴얼 에서는 DLP 폴더를 선택한 후 폴더 속성에서 파일첨부 메일발송을 활성화하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '공유 설정'  항목에 접근할 수 있습니다.
* DLP 관리의 폴더 속성에서 파일첨부 메일발송을 활성화하려면, ['DLP 설정'에서 사용자에게 파일첨부 메일발송 기능을 허용하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-dlp/dlp-3)의 절차에 따라 'SHIELD' > 'DLP 설정' 메뉴의 파일 반출 설정 탭에서 파일첨부 메일발송 설정의 사용이 선택되어 있어야 합니다.
* 파일첨부 메일발송 설정은 기본적으로 사용으로 설정되어 있습니다.
* 파일첨부 메일발송 설정은 제1계층 폴더에 대해 설정하며, 설정한 내용은 하위 폴더에 그대로 적용됩니다.
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

1. '공유 설정' > 'DLP 관리' 메뉴를 선택한 후, 다운로드를 활성화하려는 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (164).png" alt=""><figcaption></figcaption></figure>

2. 화면을 아래로 스크롤하여 폴더 속성 설정에서 파일첨부 메일발송 설정의 수정 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2475).png" alt=""><figcaption></figcaption></figure>

3. 사용 여부가 '사용 안함'으로 설정되어 있는 경우, '사용'을 선택한 후 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2476).png" alt=""><figcaption></figcaption></figure>
