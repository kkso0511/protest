---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/images-and-media/undefined-2
---

# 로그인 비밀번호의 연속 입력을 제한하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, ‘비밀번호 정책’ 메뉴에서 사용자 및 Guest가 로그인 비밀번호에 동일한 문자를 연속해서 입력하지 못하도록 제한하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 ‘보안 정책’을 사용할 수 있습니다.
* ‘LDAP 연동’을 ‘사용’으로 설정한 경우에는 ‘비밀번호 정의’를 설정할 수 없습니다.
* 비밀번호 정책은 Guest에게도 적용되지만, Connect User, LDAP 연동 및 SAML 연동으로 등록된 사용자에게는 적용되지 않습니다.
* 비밀번호 정책은 로그인 비밀번호에만 적용됩니다. 공유 링크, 파일첨부 메일발송, 업로드 요청의 비밀번호에는 적용되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '보안 정책' > '비밀번호 정책' 메뉴를 선택하고 '설정' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (724).png" alt=""><figcaption></figcaption></figure>



2. '동일 문자 연속 사용 제한'에서 '있음'을 체크하고 2\~6회 이내의 숫자를 입력하고 '저장' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (731).png" alt=""><figcaption></figcaption></figure>
