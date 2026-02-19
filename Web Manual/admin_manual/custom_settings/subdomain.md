---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/custom_settings/subdomain
---

# 사용자 로그인 페이지에 맞춤형 도메인을 설정하는 방법(미제공?)

### 개요 <a href="#a03" id="a03"></a>

사용자 페이지의 로그인 URL을 변경하면 사용자가 로그인할 때 회사코드 입력을 생략할 수 있습니다.\
이 매뉴얼에서는 '맞춤형 설정' 메뉴의 '맞춤형 도메인 설정'에서 사용자 로그인 페이지의 서브도메인을 변경하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정' 메뉴를 사용할 수 있습니다.
* 서브도메인을 등록한 후 DNS 서버에 반영되기까지 다소 시간이 소요될 수 있습니다.
* 희망하는 서브도메인명이 이미 다른 회사 ID에서 사용 중인 경우에는 서브도메인 설정을 할 수 없습니다.
* 서브도메인을 등록한 후 오류가 발생한 경우에는 다른 서브도메인명을 검토해 주십시오.
* 서브도메인을 변경하더라도 공유 링크의 URL은 변경되지 않습니다. 계속해서 서브도메인을 변경하기 전에 생성된 공유 링크에 접근할 수 있습니다.
* 서브도메인 변경은 연 1회에 한해 가능합니다. 변경에 대해서는 도입 후 문의 폼을 통해 문의해 주십시오.
* 본 매뉴얼의 절차에 따라 서브도메인을 설정한 경우, 도입 후 문의 폼을 통해 신청하면 Web 브라우저의 로그인 화면에 표시되는 배너를 비표시로 설정할 수 있습니다.
*   SSO 연동으로 IdP와 SSO를 연동하고, IdP가 제공하는 인증 정보를 사용하여 DirectCloud에 싱글 사인온하도록 설정한 경우, 본 매뉴얼의 절차에 따라 서브도메인을 설정하면 Web 브라우저의 로그인 화면에서 실수로 사용자 ID와 비밀번호를 입력하지 않도록 '사용자 ID' 및 '비밀번호' 입력란이 표시되지 않게 됩니다.

    자세한 내용은 \[Web 앱·드라이브] 타사 IdP의 사용자 ID·비밀번호로 사용자 페이지에 로그인하는 방법을 참고해 주십시오.

### 절차 <a href="#a05" id="a05"></a>

{% hint style="info" %}
**서브 도메인 설정**
{% endhint %}

1. '공유 설정' > '맞춤형 설정' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (441).png" alt=""><figcaption></figcaption></figure>



2. 'Web 도메인 맞춤형 설정'에서 맞춤형 도메인을 '서브 도메인 사용' 선택합니다.

<figure><img src="../../.gitbook/assets/image (2535).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="277">항목</th><th>설명</th></tr></thead><tbody><tr><td>맞춤형 도메인</td><td>맞춤 도메인 설정 여부를 선택할 수 있습니다.<br>서브 도메인을 설정하려면 서브 도메인 사용을 선택합니다.</td></tr><tr><td>URL</td><td>사용자 로그인 페이지의 하위 도메인을 5~30자 이내로 입력합니다.<br>사용 가능한 문자: 영문소문자, 숫자, 기호(-)</td></tr><tr><td>공통 로그인 화면(web.directcloud.net)은 접속을 차단합니다.</td><td>선택하면 일반 로그인 URL에 액세스할 수 없습니다.</td></tr></tbody></table>



3. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2536).png" alt=""><figcaption></figcaption></figure>
