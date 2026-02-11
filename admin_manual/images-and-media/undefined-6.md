---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/images-and-media/undefined-6
---

# 일정 시간 조작이 없을 때 자동 로그아웃시키는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, 로그인 설정 메뉴의 자동 로그아웃 설정에서 일정 시간 동안 조작이 없었던 사용자와 Guest를 자동으로 로그아웃하도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 자동 로그아웃은 Guest, LDAP 연동 및 SAML 연동으로 등록된 사용자에게도 적용됩니다.
* '로그인 자동종료 설정'이 '사용'으로 설정되어 있지만 로그아웃되지 않는 경우 다음과 같은 가능성이 있습니다.
  * 설정 한 시간 내에 사용자 및 게스트가 조작한경우
  * 보안 소프트웨어의 바이러스 검사 등으로 액세스가 발생한 경우
* 모바일 버전 Web 브라우저는 2024년 12월 10일 업데이트에서 베타 버전으로 제공되기 시작했습니다.
*   자동 로그아웃은 기본적으로 사용함으로 설정되어 있으며, PC 버전 Web 브라우저, PC Agent, DirectCloud 드라이브, 모바일 애플리케이션을 사용하는 경우에는 30분 동안 조작이 없으면 자동으로 로그아웃되도록 설정되어 있습니다.

    단, 모바일 버전 Web 브라우저의 자동 로그아웃은 기본적으로 꺼짐으로 설정되어 있습니다.

***

### 절차 <a href="#a05" id="a05"></a>

1. '보안 정책' > '로그인 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (747).png" alt=""><figcaption></figcaption></figure>



2. '로그인 자동종료 설정'의 '자동종료'를 '사용'으로 선택하고 다음 항목을 설정합니다.

<figure><img src="../../.gitbook/assets/image (379).png" alt=""><figcaption></figcaption></figure>

| 항목    | 설명              |
| ----- | --------------- |
| 사용    | 자동 로그아웃을 사용합니다. |
| 사용 안함 | 자동 로그아웃을 방지합니다. |



3. 자동 로그아웃되기까지의 시간을 30분, 1시간, 3시간, 6시간, 12시간, 1일, 3일, 1주, 1개월 중에서 선택합니다.

<figure><img src="../../.gitbook/assets/image (381).png" alt=""><figcaption></figcaption></figure>



4. 자동 로그아웃 설정을 적용할 애플리케이션을 PC 버전 Web 브라우저, PC Agent, DirectCloud 드라이브, 모바일 애플리케이션, 모바일 버전 Web 브라우저 중에서 선택합니다.

<figure><img src="../../.gitbook/assets/image (382).png" alt=""><figcaption></figcaption></figure>



5. '저장' 버튼을 누릅니다.

<figure><img src="../../.gitbook/assets/image (383).png" alt=""><figcaption></figcaption></figure>
