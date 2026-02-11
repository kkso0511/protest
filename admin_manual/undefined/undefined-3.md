---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined/undefined-3
---

# 업로드 가능한 파일을 확장자로 제한하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '보안 정책' > '반입 정책' 메뉴의 업로드 제한 설정에서 업로드 가능한 파일을 확장자로 제한하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 확장자 제한은 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용됩니다.
* 확장자 제한은 My Box와 Shared Box뿐만 아니라 Connect 폴더, DLP 폴더에도 적용됩니다.
* 이 매뉴얼에서 설정한 확장자 기반 업로드 제한은 일반 업로드뿐 아니라 다음 업로드 방식에도 적용됩니다.
  * 링크의 업로드 기능을 이용한 파일 업로드
  * 업로드 요청 폴더에 파일 업로드
  * 업로드 전용 메일을 통한 파일 업로드
* 이 설정은 DirectCloud 드라이브에는 적용되지 않습니다.
* 허가 목록 또는 거부 목록 중 하나만 입력할 수 있습니다.
* DirectCloud-CONNECT를 사용할 수 있는 경우, 확장자 제한의 대상에 Connect 체크박스가 표시됩니다.
* DirectCloud-SHIELD DLP를 계약한 경우, 확장자 제한의 대상에 DLP 체크박스가 표시됩니다.
* Warm Storage를 사용할 수 있다면 확장자 제한의 대상에 Warm Storage 체크박스가 표시됩니다.
* Cold Storage를 계약한 경우, 확장자 제한의 대상에 Cold Storage 체크박스가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '보안 정책' > '반입 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1637).png" alt=""><figcaption></figcaption></figure>



2. 업로드 제한 설정의 '확장자 제한'에서 '사용'을 선택합니다.\
   확장자 제한 설정 필드가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1638).png" alt=""><figcaption></figcaption></figure>



3. 범위, 허가할 확장자, 금지할 확장자를 설정하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1639).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="165">항목</th><th>설명</th></tr></thead><tbody><tr><td>범위</td><td>확장자 및 파일 크기 제한을 적용하기 위해 "My Box", "Shared Box"를 선택할 수 있습니다.</td></tr><tr><td>허가할 확장자</td><td>업로드를 허용할 파일 형식의 확장자를 입력합니다.<br>쉼표(,)로 구분하여 여러 확장자를 입력할 수 있습니다.<br>허용 목록 또는 거부 목록 중 하나에 입력할 수 있습니다.<br>입력 예: docx, xlsx, pptx, png, pdf, txt</td></tr><tr><td>금지할 확장자</td><td>업로드를 허용하지 않는 파일 형식의 확장자를 입력합니다.<br>쉼표(,)로 구분하여 여러 확장자를 입력할 수 있습니다.<br>허용 목록 또는 거부 목록 중 하나에 입력할 수 있습니다.<br>입력 예: exe, zip, xlsm, docm</td></tr></tbody></table>
