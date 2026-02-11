---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/sso/microsoft-entra-id-sso
---

# Microsoft Entra ID와 SSO를 연결하는 방법

### 개요 <a href="#a03" id="a03"></a>

Microsoft Entra ID를 사용하면 Office 365, Intune, Dynamics CRM Online과 같은 Microsoft 클라우드 서비스뿐만 아니라 다양한 클라우드 서비스를 안전하게 인증할 수 있습니다.\
이 문서에서는 Microsoft Entra ID와 SAML 인증을 통해 SSO와 협력하여 DirectCloud에 로그인하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Microsoft 및 기타 회사에서 제공하는 서비스 및 사용자 인터페이스(UI) 등은 예고 없이 변경될 수 있습니다. 이에 따라 본 기사에서 사용하고 있는 화면의 명칭 등도 바뀔 가능성이 있습니다. 이 경우 제공된 서비스나 기능, UI 등에 맞춰 본 기사의 절차를 수행하도록 하십시오.
* Azure Active Directory의 이름은 2023년 10월 1일에 Microsoft Entra ID로 변경되었습니다.
* Microsoft Entra ID에 로그인하기 위한 MFA(다중 요소 인증)와 같은 인증 방법은 Microsoft Entra ID 설정에 따라 다릅니다. 절차를 시작하기 전에 확인해야 합니다.
* SSO에서 작동하는 Microsoft Entra ID의 계정 상태가 '사용 안 함'인 경우 DirectCloud에 SSO 로그인할 수 없습니다.
* 일반 사용자가 SSO 로그인을 허용하려면 먼저 Microsoft 365 관리 센터에서 사용자 및 그룹을 관리하는 관리자 역할이 할당된 사용자로 Microsoft에 로그인하고 사용 권한을 수락해야 합니다. .\
  사용자 및 그룹을 관리할 수 있는 관리자 역할에는 "사용자 관리자" 및 "그룹 관리자"가 있습니다.\
  관리자 역할에 대한 자세한 내용은 Microsoft 설명서를 참조하십시오.

### 절차 <a href="#a05" id="a05"></a>

#### Microsoft Entra 관리 센터에서 SSO 연합 준비 <a href="#junbi" id="junbi"></a>

Microsoft Entra 관리 센터에서 Microsoft에서 제공하는 SAML 인증을 위한 XML 데이터를 다운로드합니다.

1. [Microsoft Entra 관리 센터](https://entra.microsoft.com/) 에 로그인합니다.
2. 왼쪽 메뉴에서 앱 > 앱 등록을 클릭합니다.\
   앱 등록 페이지가 표시됩니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjUn)

3. 상단 메뉴에서 엔드포인트를 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjU0)

엔드포인트 목록이 표시됩니다.

4. 페더레이션 메타데이터 문서의 오른쪽에 있는 클립보드에 복사 단추를 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjWP)

메타데이터 URL이 복사됩니다.

5. 웹 브라우저의 주소 입력란에 4단계에서 복사한 URL을 붙여넣습니다.\
   XML 형식의 데이터가 표시됩니다.
6. 웹 브라우저에 표시된 데이터를 마우스 오른쪽 버튼으로 클릭하고 다른 이름으로 저장을 선택합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjXX)

7. 모든 폴더에 XML 파일로 저장합니다.

#### DirectCloud에서 Microsoft Entra ID와 협력

DirectCloud에서 Microsoft Entra ID와 함께 작동하도록 설정합니다.

1. [DirectCloud 관리 페이지](https://boxmanager.directcloud.jp/) 에서 사용자 > SSO 연동 메뉴를 선택하고 SAML 탭을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001wjVd)

2. 「SAML2.0 연계」의 「사용한다」를 체크합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001whqQ)

3. IdP 설정에서 Microsoft Entra ID를 선택합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001wjc5)

4. 화면을 아래로 스크롤하여 SAML 인증서 설정을 표시한 다음 파일 선택 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004cyqW)

5. [Microsoft Entra 관리 센터에서 SSO 연결 준비를](https://help.directcloud.jp/s/article/operation-of-administrator-function12002#junbi) 위해 저장한 XML 파일을 선택합니다.
6. 다음 설정을 지정하고 저장 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjY6)

| 품목        | 설명                                                                                                                                                                                                                       |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 로그인 계정    | <p>SSO 연결되지 않은 사용자가 로그인을 허용할지 여부를 설정합니다.</p><ul><li>IdP 계정만 사용<br>IdP 사용자만 사용할 수 있으며 사용자 > 사용자 관리 메뉴에 등록된 사용자는 사용할 수 없습니다.</li><li>IdP 및 DirectCloud 계정 모두 사용 IdP<br>사용자와 사용자 > 사용자 관리 메뉴에 등록된 사용자가 모두 활성화됩니다.</li></ul> |
| 로그아웃 시 처리 | <p>사용자 페이지에서 로그아웃할 때 IdP에서 로그아웃할지 여부를 설정합니다.</p><ul><li>DirectCloud만 로그아웃<br>IdP에서 로그아웃되지 않습니다.</li><li>DirectCloud와 IdP 모두에서 로그아웃<br>IdP에서도 연동하여 로그아웃됩니다.</li></ul>                                                     |
| 용량        | <p>IdP 사용자에게 할당할 내 상자의 용량을 계약 계획의 총 스토리지 용량 범위 내에서 설정합니다.<br>공유 폴더의 용량은 포함되지 않습니다.</p><ul><li>사용 가능한 문자: 1개 이상의 반각 숫자(단위: MB)</li><li>1024MB는 1GB로 변환됩니다.</li></ul>                                                      |

7. 상태에 유효( _고유 테넌트 ID_ )가 표시되는지 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001wjgv)

#### DirectCloud 사용자 로그인 화면에서 사용 권한 수락

인증 테스트를 위해 DirectCloud 사용자 페이지에 SSO로 로그인합니다.\
요청한 액세스를 허용하려면 먼저 Microsoft Entran Management Center에서 관리자 역할이 할당된 사용자로 로그인해야 합니다.\
일단 이 화면에서 사용 권한을 수락하면 이후 일반 사용자가 SSO 로그인할 수 있습니다.

1. DirectCloud 사용자 페이지의 로그인 화면을 표시합니다.\
   DirectCloud 관리 페이지의 사용자 > SSO 연동 메뉴에서 SAML 탭을 표시하고 인증 테스트의 로그인 화면으로 이동을 클릭하여 사용자 페이지의 로그인 화면을 볼 수 있습니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjYV)

2. 로그인 화면에서 "SSO로 로그인"을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjYk)

SSO로 로그인 화면이 표시됩니다.\
회사 ID가 설정된 경우 4단계로 진행합니다.

3. 회사 ID를 입력하고 확인 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjYp)

Microsoft Entra ID에 로그인하는 상황에 따라 다음 단계 중 하나를 따르십시오.❶ Microsoft Entra ID에 로그인하지 않은 경우 계정 선택 화면이 표시됩니다. 4단계로 진행합니다.❷ "관리자 승인 필요"라는 화면이 나타나면 관리자 역할이 할당되지 않은 사용자로 로그인한 것입니다. 이 경우 "관리자 계정이있는 경우 해당 계정으로 로그인합니다."를 클릭하면 "계정 선택"화면이 나타납니다. 4단계로 진행합니다.❸ Microsoft Entra ID에 관리자 역할이 할당된 사용자로 로그인한 경우 요청된 사용 권한 화면이 표시됩니다. 5단계로 진행합니다.

4. SSO로 로그인 Microsoft Entra ID의 사용자를 클릭하고 인증을 받고 로그인합니다.\
   Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자를 선택합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjcN)

5. 요청된 사용 권한 화면이 표시되면 조직 대리인으로 동의함을 선택하고 수락 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMQ8000003zag1)

사용자 페이지에 로그인합니다.

6. DirectCloud 사용자 페이지에서 왼쪽 상단의 사용자 이름을 클릭하여 설정 화면을 표시하고 Microsoft Entra ID와 연결된 사용자로 로그인했는지 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001IhF\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sjcX)
