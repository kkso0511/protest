---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/sso/google-workspace-sso
---

# Google Workspace와 SSO를 연결하는 방법

### 개요 <a href="#a03" id="a03"></a>

Google에서 제공하는 그룹웨어의 Google Workspace와 SSO를 사용하면 Gmail, Google 드라이브, Google 행아웃, Google 캘린더 등의 애플리케이션뿐만 아니라 다양한 클라우드 서비스를 안전하게 인증할 수 있습니다.\
이 섹션에서는 Google Workspace와 SAML 인증을 통해 SSO와 협력하여 DirectCloud에 로그인하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Google 및 기타 회사에서 제공하는 서비스 및 사용자 인터페이스(UI) 등은 예고 없이 변경될 수 있습니다. 이에 따라 본 기사에서 사용하고 있는 화면의 명칭 등도 바뀔 가능성이 있습니다. 이 경우 제공된 서비스나 기능, UI 등에 맞춰 본 기사의 절차를 수행하도록 하십시오.
* Google 관리 콘솔 설정을 변경하면 변경 사항이 반영되기까지 시간이 걸릴 수 있습니다.
* Google Workspace에 로그인하기 위한 2단계 인증과 같은 인증 방법은 Google 관리 콘솔 설정에 따라 다릅니다. 절차를 시작하기 전에 확인해야 합니다.
* DirectCloud와의 SSO 연계에 관한 사양에 대해서는, SSO 제휴에 관한 사양 및 주의 사항을 참조해 주세요.

### 절차 <a href="#a05" id="a05"></a>

#### DirectCloud에서 Google Workspace와 협력하기 위한 정보 얻기 <a href="#get_information" id="get_information"></a>

Google Workspace와 SSO를 사용하려면 맞춤 SAML 앱을 만들어야 합니다.\
여기에서는 DirectCloud 관리 페이지에 로그인하여 Google Workspace에서 맞춤 SAML 앱을 만드는 데 필요한 정보를 검색합니다.

1. [DirectCloud 관리 페이지](https://boxmanager.directcloud.jp/) 에서 사용자 > SSO 연동 메뉴를 선택하고 SAML 탭을 클릭합니다.

![001\_b\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AHjC)

2. 「SAML2.0 연계」의 「사용한다」를 체크합니다.

![002\_t\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002ACMz)

3. IdP 설정에서 Google Workspace를 선택하여 표시된 정보를 확인합니다.\
   이 정보는 [Google Admin에서 맞춤 SAML 앱을 만들고 맞춤](https://help.directcloud.jp/s/article/operation-of-administrator-function12005#create_custom_application) SAML 앱을 설정하는 데 필요합니다.

![002\_t\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AL8T)

| 품목                                                                    | 설명                                                                                                                                |
| --------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| ACS URL                                                               | <p>ACS (Assertion Consumer Service) URL은 사용자 SAML 인증이 완료된 후 리디렉션되는 URL입니다.<br>IdP에서 보낸 SAML 응답을 받는 URL로 맞춤 SAML 앱에 설정해야 합니다.</p>  |
| 엔티티 ID                                                                | <p>응용 프로그램을 식별하는 데 사용되는 고유 문자열입니다. 여러 SAML 앱에서 동일한 문자열을 사용할 수 없습니다.<br>Google Workspace에서 다운로드하는 SAML 메타데이터는 EntityID로 표시됩니다.</p> |
| 시작 URL                                                                | DirectCloud 사용자 페이지에서 SSO 로그인하여 SAML 인증을 시작하는 대신 관리 콘솔에서 만든 사용자 지정 SAML 앱에서 SAML 인증을 시작하는 데 필요한 정보입니다.                            |

#### Google Admin에서 맞춤 SAML 앱 만들기 <a href="#create_custom_-application" id="create_custom_-application"></a>

Google에 관리자 계정으로 로그인하여 맞춤 SAML 앱을 만듭니다.

**맞춤 SAML 앱 만들기 시작**

1. [Google Admin](https://admin.google.com/) 에 관리자 계정으로 로그인합니다.\
   Google Workspace 관리 콘솔이 표시됩니다.
2. 메뉴 아이콘을 클릭하고 앱 > 웹 및 모바일 앱을 선택합니다.

![004\_tb\_70%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AURt)

3. 앱 추가 > 맞춤 SAML 앱 추가를 선택합니다.

![005\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AUbZ)

사용자 정의 SAML 앱 추가 화면이 표시됩니다.

**맞춤 SAML 앱 이름 설정**

1. 앱 이름에 맞춤 SAML 앱의 이름을 영숫자로 입력합니다.

![006\_t\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002ATXS)

2. 필요한 경우 '설명'에 앱 설명을 입력합니다.\
   또한 필요에 따라 '앱 아이콘'에서 카메라 버튼을 클릭하고 앱에 설정할 이미지 데이터를 선택합니다.

![007\_t\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002ARx4)

3. 계속 버튼을 클릭합니다.

![008\_t\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AVEH)

Google ID 공급자 세부 정보 페이지가 표시됩니다.

**Google ID 공급자 세부정보로 메타데이터 다운로드**

1. 메타데이터 다운로드 버튼을 클릭합니다.

![009\_t\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AVML)

메타데이터 XML 파일이 다운로드됩니다.\
이 파일은 DirectCloud의 SAML 설정에서 "SAML 인증서"로 지정됩니다.

2. 계속 버튼을 클릭합니다.\
   서비스 공급자 세부사항 페이지가 표시됩니다.

![010\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AVRB)

**서비스 제공업체의 고급 설정**

1. 'ACS URL'과 '엔티티 ID'에 [DirectCloud에서 Google Workspace와 연동하기 위한 정보 얻기](https://help.directcloud.jp/s/article/operation-of-administrator-function12005#get_information) 에서 확인한 정보를 입력합니다.

![011\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002ATFj)

2. 필요한 경우 '시작 URL'에 [DirectCloud에서 Google Workspace와 연결하기 위한 정보 얻기](https://help.directcloud.jp/s/article/operation-of-administrator-function12005#get_information) 에서 확인한 정보를 입력합니다.

![012\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AUtK)

3. 화면을 아래로 스크롤하고 이름 ID 형식에서 EMAIL을 선택하고 이름 ID에서 Basic Information > Primary email을 선택합니다.

![013\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AVuD)

4. 계속 버튼을 클릭합니다.

![014\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AVxR)

속성 매핑 페이지가 표시됩니다.

**속성 매핑**

1. 매핑 추가 버튼을 클릭합니다.

![015\_t\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002ATPP)

DirectCloud 항목과 Google Workspace 항목을 연결하기 위한 설정 입력란이 추가됩니다.

2. 'Google Directory 속성'과 '앱 속성'을 다음과 같이 연결합니다.

![016\_t\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AYnF)

| Google Directory 속성 | 앱 속성      |
| ------------------- | --------- |
| Primary email       | email     |
| First name          | firstname |
| 마지막 이름              | lastname  |

3. 마침 버튼을 클릭합니다.

![017\_t\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AYfB)

작성한 맞춤 SAML 앱 페이지가 표시됩니다.

#### DirectCloud에서 SSO 연동 설정하기

DirectCloud에서 Google Workspace와 SSO를 사용하도록 설정합니다.

1. [DirectCloud 관리 페이지](https://boxmanager.directcloud.jp/) 에서 사용자 > SSO 연동 메뉴를 선택하고 SAML 탭을 클릭합니다.

![004\_tb\_70%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AZpl)

2. 「SAML2.0 연계」의 「사용한다」를 체크합니다.

![004\_tb\_70%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002Aa7V)

3. IdP 설정에서 Google Workspace를 선택합니다.

![020\_t\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AaCL)

4. 화면을 아래로 스크롤하여 'SAML 인증서' 설정을 표시한 다음 '파일 선택' 버튼을 클릭하여 [Google Admin에서 맞춤 SAML 앱 만들기](https://help.directcloud.jp/s/article/operation-of-administrator-function12005#create_custom_%20application) 에서 저장한 메타데이터의 XML 파일을 선택합니다.

![021\_t\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004d0Ne)

5. 다음 설정을 지정하고 저장 버튼을 클릭합니다.

![022\_t\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AUuw)

| 품목        | 설명                                                                                                                                                                                                                       |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 로그인 계정    | <p>SSO 연결되지 않은 사용자가 로그인을 허용할지 여부를 설정합니다.</p><ul><li>IdP 계정만 사용<br>IdP 사용자만 사용할 수 있으며 사용자 > 사용자 관리 메뉴에 등록된 사용자는 사용할 수 없습니다.</li><li>IdP 및 DirectCloud 계정 모두 사용 IdP<br>사용자와 사용자 > 사용자 관리 메뉴에 등록된 사용자가 모두 활성화됩니다.</li></ul> |
| 로그아웃 시 처리 | <p>사용자 페이지에서 로그아웃할 때 IdP에서 로그아웃할지 여부를 설정합니다.<br>Google Workspace와 SSO를 사용하는 경우 DirectCloud에서 로그아웃할 때 IdP에서 동시에 로그아웃할 수 없습니다. 설정은 'DirectCloud 전용 로그아웃'으로 고정되므로 이 항목은 회색으로 표시됩니다.</p>                                     |
| 용량        | <p>IdP 사용자에게 할당할 내 상자의 용량을 계약 계획의 총 스토리지 용량 범위 내에서 설정합니다.<br>공유 폴더의 용량은 포함되지 않습니다.</p><ul><li>사용 가능한 문자: 1개 이상의 반각 숫자(단위: MB</li><li>1024MB는 1GB로 변환됩니다.</li></ul>                                                       |

"저장되었습니다."라는 메시지가 나타납니다.

6. 페이지를 다시 로드하고 상태에 유효( _엔터티 ID_ )가 표시되는지 확인합니다.

![023\_tb\_60%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AY2U)

#### 맞춤 SAML 앱 상태 사용

작성한 맞춤 SAML 앱의 상태를 사용으로 설정합니다.

1. [Google Admin](https://admin.google.com/) 에 관리자 계정으로 로그인합니다.\
   Google Workspace 관리 콘솔이 표시됩니다.
2. 메뉴 아이콘을 클릭하고 앱 > 웹 및 모바일 앱을 선택합니다.

![024\_tb\_70%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AbwP)

3. 앱 목록에서 [Google Admin에서 맞춤 SAML 앱 만들기](https://help.directcloud.jp/s/article/operation-of-administrator-function12005#create_custom_%20application) 에서 만든 앱을 클릭합니다.

![025\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AZbH)

4. 사용자 액세스 오른쪽 상단의 ∨ 버튼을 클릭합니다.

![026\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AY7K)

서비스 상태가 표시됩니다.

5. 켜기(모든 사용자)를 선택하고 저장을 클릭합니다.

![027\_tb\_65%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AcMD)

서비스 상태가 저장되면 "서비스 상태를 업데이트했습니다."라는 메시지가 표시됩니다.

#### 사용자 페이지에서 SSO 로그인

DirectCloud 사용자 페이지에서 SSO로 로그인합니다.

1. 사용자 페이지의 로그인 화면을 표시합니다.\
   DirectCloud 관리 페이지의 "사용자" > "SSO 연동" 메뉴에서 "SAML" 탭을 표시하고 "인증 테스트"의 "로그인 화면으로 이동"을 클릭하면 사용자 페이지의 로그인 화면을 볼 수 있습니다.
2. SSO로 로그인을 클릭합니다.

![028\_t\_45%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AcUH)

SSO로 로그인 화면이 표시됩니다.\
회사 ID가 설정된 경우 4단계로 진행합니다.

3. 회사 ID를 입력하고 확인 버튼을 클릭합니다.

![029\_rtb\_45%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002Acu5)

Google Workspace와 SSO를 사용하는 회사 ID의 경우 Google Workspace의 '계정 선택' 화면이 표시됩니다.

4. SSO로 로그인하려는 Google 계정을 클릭하고 인증을 받고 로그인합니다.

![030\_tb\_75%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002AY47)

5. DirectCloud 사용자 페이지에서 왼쪽 상단의 사용자 이름을 클릭하여 '설정' 화면을 표시하고 Google Workspace와 연결된 사용자로 로그인했는지 확인합니다.

![031\_tb\_75%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IkT\&feoid=00N2w00000JMb2T\&refid=0EMQ8000002Ad29)
