---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-14/directcloud
---

# DirectCloud 공통 사양

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud의 모든 애플리케이션에 공통되는 사양에 대해 설명합니다.

***

### 설명 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**데이터의 저장 및 표시와 관련된 사양**
{% endhint %}

| 한 회사 ID로 저장할 수 있는 폴더 및 파일 수의 최대값(이론치)                 | 무제한                                                                                                                                                              |
| ----------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1개 폴더에 저장할 수 있는 폴더 및 파일 수의 최대값(이론값)                   | <p>· 파일: 무제한<br>· 폴더: 최대 238,328개</p>                                                                                                                            |
| 1개 폴더에 저장할 수 있는 폴더 및 파일 수의 최대값(권장)                    | 폴더와 파일을 합쳐 2,000개 이내                                                                                                                                             |
| 한 번에 작업할 수 있는 폴더 및 파일의 총합(권장)                         | 폴더와 파일을 합쳐 1,000개 이내                                                                                                                                             |
| 1개 폴더에서 표시할 수 있는 폴더 및 파일 수의 최대값(이론치)                  | <ul><li>웹 애플리케이션, PC 애플리케이션(Windows, Mac), 모바일 애플리케이션(iOS, Android): 무제한</li><li>DirectCloud 드라이브(Windows, Mac):<br>폴더와 파일의 총 5,000개 이내</li></ul>                |
| 데이터 저장 위치                                             | <ul><li>도쿄 리전의 가용 영역(AZ) 3곳(Amazon S3)</li><li>오사카 지역 또는 싱가포르 지역(유료 옵션)</li></ul>                                                                                |
| 저장 대상                                                 | <ul><li>파일(실체)</li><li>디렉토리 정보의 데이터, 서버 구성의 데이터 등(스냅샷, 일별로 10세대)</li></ul>                                                                                       |
| 장애 발생 시 복구 및 업무 연속성 계획(BCP, Business Continuity Plan) | <ul><li>도쿄 리전: <br>· 대응 가능(장애가 발생한 AZ는 다른 AZ로 자동 전환)</li><li>오사카 리전, 싱가포르 리전: <br>· 파일 실체는 실시간 다운로드 가능<br>· 리스토어는 불가(일 단위로 저장된 스냅샷을 이용한 데이터베이스 롤백은 가능)</li></ul> |



{% hint style="warning" %}
**네트워크 관련 사양**
{% endhint %}

**\[네트워크 정보]**

| 액세스 대상 IP 주소 | <p>변동<br><br><strong>NOTE</strong><br>부하 분산을 위해 접속 대상 IP 주소는 예고 없이 비정기적으로 변경될 수 있습니다.<br>방화벽이나 프록시 서버를 사용하는 경우의 설정 방법은 ‘포트 번호와 도메인 접근 제어에 대해’ 항목을 참고하시기 바랍니다.</p> |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 통신 프로토콜      | TCP、HTTPS                                                                                                                                                         |
| 포트 번호        | 443                                                                                                                                                               |
| 통신 암호화 프로토콜  | TLS1.2                                                                                                                                                            |



**\[포트 번호 및 도메인 액세스 제어 정보]**

방화벽이나 프록시 서버를 사용하는 환경에서 DirectCloud를 사용하려면 액세스하려는 네트워크의 방화벽이나 프록시 서버에서 포트 번호 443 및 다음 도메인에 대한 통신을 허용하도록 구성해야 합니다. .

* 와일드카드를 사용할 수 있는 경우\
  \*. directcloud.net\
  \*. directcloud.jp\
  \*. amazonaws.com\
  \*.cloudfront.net
* 와일드카드를 사용할 수 없는 경우
  *   사내 구성원이 관리 페이지 설정이나 파일의 기본적인 작업을 수행하기 위해 필요한 도메인

      | 도메인                                                                                                                                                                                                                                  | 용도                                             |
      | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------- |
      | <p>· api.directcloud.jp(일본)<br>· api.directcloud.jp(한국)</p>                                                                                                                                                                          | <p>· API 서버 접근<br>· DirectCloud 내부의 API 통신</p> |
      | boxmanager.directcloud.jp                                                                                                                                                                                                            | DirectCloud 관리 페이지 접근                          |
      | <p>· cdn.directcloud.jp(일본)<br>· cdn.directcloud.net(한국)<br>· officebox-tokyo.s3-ap-northeast-1.amazonaws.com<br>· d3ishwaaf5up45.cloudfront.net<br>· s3-r-w.ap-northeast-1.amazonaws.com<br>· s3-w.ap-northeast-1.amazonaws.com</p> | 폴더 및 파일 다운로드                                   |
      | link.directcloud.jp                                                                                                                                                                                                                  | 링크 생성                                          |
      | officebox-tokyo.s3.ap-northeast-1.amazonaws.com                                                                                                                                                                                      | CSV 파일 내보내기                                    |
      | <p>· officebox-osaka-slv.s3.ap-northeast-3.amazonaws.com(오사카 리전)<br>· officebox-tokyo-slv.s3-ap-southeast-1.amazonaws.com(싱가포르 리전)</p>                                                                                               | 재해 대비 및 원격지 백업                                 |
      | s3.ap-northeast-1.amazonaws.com                                                                                                                                                                                                      | 프로필 설정 이미지 표시                                  |
      | <p>· s3-r-w.ap-northeast-1.amazonaws.com<br>· s3-w.ap-northeast-1.amazonaws.com</p>                                                                                                                                                  | DirectCloud 드라이브 자동 업데이트                       |
      | safeupdate.s3.amazonaws.com                                                                                                                                                                                                          | PC 애플리케이션 자동 업데이트                              |
      | sp.directcloud.jp                                                                                                                                                                                                                    | DirectCloud 드라이브 환경 진단                         |
      | temp-officebox-tokyo.s3.ap-northeast-1.amazonaws.com                                                                                                                                                                                 | 승인 워크플로를 통한 파일 다운로드                            |
      | thumb.directcloud.jp                                                                                                                                                                                                                 | 썸네일 생성                                         |
      | thumbnail-officebox-tokyo.s3.ap-northeast-1.amazonaws.com                                                                                                                                                                            | 썸네일 표시                                         |
      | update.directcloud.jp                                                                                                                                                                                                                | DirectCloud-SHIELD IRM 설치                      |
      | uploader.directcloud.jp                                                                                                                                                                                                              | 폴더 및 파일 업로드                                    |
      | viewer.directcloud.jp                                                                                                                                                                                                                | 파일 미리보기                                        |
      | <p>web.directcloud.jp(일본)<br>web.directcloud.net(한국)</p>                                                                                                                                                                             | DirectCloud PC 버전 웹 애플리케이션 사용                  |
      | <p>webm.directcloud.jp(일본)<br>webm.directcloud.net(한국)</p>                                                                                                                                                                           | 모바일 버전 웹 애플리케이션 사용                             |
  *   Guest가 파일의 기본적인 작업을 수행하기 위해 필요한 도메인

      | <p>api.directcloud.jp</p><p>api.directcloud.net</p><p>link.directcloud.jp</p><p>officebox-tokyo.s3-ap-northeast-1.amazonaws.com</p><p>temp-officebox-tokyo.s3.ap-northeast-1.amazonaws.com</p><p>cdn.directcloud.jp</p><p>cdn.directcloud.net</p><p>officebox-tokyo.s3-ap-northeast-1.amazonaws.com</p><p>d3ishwaaf5up45.cloudfront.net</p><p>update.directcloud.jp</p><p>uploader.directcloud.jp</p><p>viewer.directcloud.jp</p><p>s3.ap-northeast-1.amazonaws.com</p><p>thumb.directcloud.jp</p><p>thumbnail-officebox-tokyo.s3.ap-northeast-1.amazonaws.com</p><p>s3-r-w.ap-northeast-1.amazonaws.com</p><p>s3-w.ap-northeast-1.amazonaws.com</p><p>safeupdate.s3.amazonaws.com</p><p>web.directcloud.jp</p><p>web.directcloud.net</p><p>webm.directcloud.jp</p><p>webm.directcloud.net</p> |
      | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  *   공유 링크에 액세스하는 데 필요한 도메인

      | <p>api.directcloud.net </p><p>api.directcloud.net </p><p>link.directcloud.net </p><p>cdn.directcloud.net </p><p>cdn.directcloud.net </p><p>viewer.directcloud.net </p><p>uploader.directcloud.net</p> |
      | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  *   업로드 요청에 액세스하기 위해 필요한 도메인

      | <p>api.directcloud.jp</p><p>api.directcloud.net</p><p>uploader.directcloud.jp</p><p>web.directcloud.jp</p><p>web.directcloud.net</p> |
      | ------------------------------------------------------------------------------------------------------------------------------------ |
  *   DirectCloud 드라이브 환경 진단을 이용하기 위해 필요한 도메인

      | sp.directcloud.jp |
      | ----------------- |



{% hint style="warning" %}
**재해 대비·원격지 백업 사이트에 관한 사양**
{% endhint %}

DirectCloud의 유료 옵션인 ‘재해 대비·원격지 백업’을 계약한 경우, ‘재해 대비·원격지 백업’ 사이트에 로그인하여 다음 파일을 다운로드할 수 있습니다.

* ‘Shared Box’메뉴 하위에 저장된 파일
* ‘Connect’ 메뉴 하위의 자사에서 생성한 폴더에 저장된 파일
* ‘Warm Storage’ 메뉴 하위에 저장된 파일

{% hint style="info" %}
**NOTE**\
일상적인 상황에서는 Warm Storage 다운로드 기능을 계약한 경우에만 다운로드가 가능합니다.\
비상 시에는 Warm Storage 다운로드 기능을 계약하지 않은 경우에도 다운로드가 가능합니다.
{% endhint %}

계약 담당 관리자와 일반 관리자는 평상시와 비상시에 관계없이 ‘재해 대비·원격지 백업’ 사이트에 로그인할 수 있습니다.

<table data-header-hidden><thead><tr><th width="525"></th><th></th></tr></thead><tbody><tr><td>오사카 리전, 싱가포르 리전이 도쿄 리전의 Amazon S3와 동기화되는 시간대</td><td>실시간</td></tr><tr><td>오사카 리전, 싱가포르 리전이 도쿄 리전의 데이터베이스와 동기화되는 시간대</td><td>매일 오전 4:00~6:00 사이</td></tr><tr><td>‘재해 대비·원격지 백업’ 사이트에 접근 가능한 애플리케이션</td><td>Web 브라우저</td></tr><tr><td>‘재해 대비·원격지 백업’ 사이트에서 가능한 작업</td><td>파일 다운로드</td></tr><tr><td>‘재해 대비·원격지 백업’ 사이트에서 사용자에게 적용 가능한 접근 제한</td><td><ul><li>IP 주소 제한</li><li>이중 인증(이메일)</li></ul></td></tr></tbody></table>



{% hint style="warning" %}
**기타 사양**
{% endhint %}

| DirectCloud와의 SSO 연동 및 송신 메일 서버 설정 시 접근 원 IP 주소 | 54.64.42.47                                                               |
| ----------------------------------------------- | ------------------------------------------------------------------------- |
| 비밀번호 암호화 알고리즘                                   | SHA-256                                                                   |
| 파일 암호화 방식                                       | AES-256                                                                   |
| 폴더 계층 한도                                        | <p>최대 65계층<br>※ 폴더 일괄 등록 시 60계층</p>                                       |
| 액세스 토큰 유효 기간                                    | <p>60일<br>※ DirectCloud 드라이브의 경우, 유효 기간 10일 이내에 조작이 이루어지면 액세스 토큰이 갱신됨</p> |
| 송신 메일 서버 연동                                     | <p>Gmail, Exchange Online: OAuth 연동<br>그외: SMTP 연동</p>                    |
| 송신 도메인 인증                                       | SPF, DKIM, DMARC 지원                                                       |
| 지원 언어                                           | 일본어, 영어, 한국어                                                              |
