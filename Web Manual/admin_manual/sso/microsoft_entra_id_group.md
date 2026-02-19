---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/sso/microsoft_entra_id_group
---

# Microsoft Entra ID 그룹 정보를 가져오는 방법

### 개요 <a href="#a03" id="a03"></a>

Microsoft Entra ID를 사용하면 Office 365, Intune, Dynamics CRM Online과 같은 Microsoft 클라우드 서비스뿐만 아니라 다양한 클라우드 서비스를 안전하게 인증할 수 있습니다.\
이 절에서는 SSO에서 작동하는 Microsoft Entra ID에서 사용자 목록 외에도 그룹 정보를 검색하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Microsoft 및 기타 회사에서 제공하는 서비스 및 사용자 인터페이스(UI) 등은 예고 없이 변경될 수 있습니다. 이에 따라 본 기사에서 사용하고 있는 화면의 명칭 등도 바뀔 가능성이 있습니다. 그 경우, 제공되고 있는 서비스나 기능, UI등에 맞추어, 이 기사를 실행하도록 해 주세요.
* Azure Active Directory의 이름은 2023년 10월 1일에 Microsoft Entra ID로 변경되었습니다.
* Microsoft Entra ID에 로그인하기 위한 MFA(다중 요소 인증)와 같은 인증 방법은 Microsoft Entra ID 설정에 따라 다릅니다. 절차를 시작하기 전에 확인해야 합니다.
* Microsoft Entra ID와의 연동은 매시간 동기화 처리를 수행하여 사용자 목록을 검색합니다. 동기화할 횟수나 시간을 변경할 수 없습니다.
* 일단 사용자 목록 검색이 설정되면 사용자 목록 검색에 실패하면 매 시간마다 재시도 처리가 수행됩니다. 첫 번째 재시도 처리가 실패하면 "사용자 목록 검색 실패 알림"이라는 제목의 알림 메일이 전송됩니다.
* Microsoft Entra ID로 사용자가 속한 그룹이 변경되면 시간별 동기화 프로세스를 통해 연결된 DirectCloud 사용자도 변경된 그룹으로 이동합니다.\
  또한 Microsoft Entra ID에서 그룹 이름과 같은 그룹 정보가 변경된 경우에도 마찬가지로 시간별 동기화 프로세스를 통해 DirectCloud에 반영됩니다.
* 사용자 > 사용자 관리 메뉴에서 사용자의 상태를 사용 안함으로 변경하여 사용자별로 DirectCloud에 대한 로그인을 제한할 수 있습니다.
* SSO에서 작동하는 Microsoft Entra ID의 계정 상태가 '사용 안 함'인 경우 '사용자 그룹 정보 가져오기'는 DirectCloud에 사용자를 가져오지만 잘못된 계정으로 DirectCloud에 SSO 로그인할 수는 없습니다.
* Microsoft Entra ID 그룹 유형에 따라 DirectCloud 기능이 제한되지 않습니다.
* UPN(User Principal Name, User Principal Name)은 Microsoft Active Directory 등에서 사용자 식별에 사용되는 'User Name@Domain Name' 형식의 로그인 이름입니다. Active Directory에서는 일반적으로 전자 메일 주소를 UPN으로 설정하지만 반드시 일치하는 것은 아닙니다.\
  DirectCloud에서는 사용자의 UPN이 이메일 주소와 일치하는지 확인할 수 없습니다.
* 이 문서의 단계에서 사용자 목록을 얻으면 사용자 > 사용자 관리 메뉴에 캡처된 사용자의 사용자 ID가 Microsoft Entra 관리 센터에서 관리되는 사용자의 사용자 주체 이름과 연결됩니다. .
* Microsoft Entra 관리 센터에서 관리하는 사용자의 속성에서 메일에 전자 메일 주소가 설정되어 있는 경우 사용자 주체 이름 외에도 해당 전자 메일 주소로 DirectCloud에 SSO 로그인할 수 있습니다. 합니다.\
  이 경우 처음 이메일 주소로 SSO 로그인했을 때 사용자 > 사용자 관리 메뉴에 이 문서의 단계에서 얻은 '#EXT#'이 포함된 사용자 주체 이름의 사용자 ID 외에 주소의 사용자 ID가 추가됩니다.\
  결과적으로 DirectCloud에는 두 개의 ID가 추가되지만 Microsoft Entra 관리 센터에서는 단일 사용자로 관리됩니다.
* Microsoft Entra 관리 센터에서 외부 사용자를 초대한 경우에는 속성의 메일에 외부 사용자의 이메일 주소가 설정됩니다.\
  DirectCloud에 SSO 로그인하는 경우 Microsoft 계정 선택 화면에서 이 이메일 주소를 지정해야 합니다.
* Microsoft Entra ID 그룹 정보를 얻으려면 Microsoft Entra 관리 센터에서 사용자 및 그룹을 관리하는 관리자 역할이 할당된 사용자로 Microsoft에 로그인하고 사용 권한을 수락해야 합니다.\
  사용자 및 그룹을 관리할 수 있는 관리자 역할에는 "사용자 관리자" 및 "그룹 관리자"가 있습니다.\
  관리자 역할에 대한 자세한 내용은 Microsoft 설명서를 참조하십시오.

### 절차 <a href="#a05" id="a05"></a>

#### Microsoft Entra 관리 센터에서 SSO 연합 준비 <a href="#junbi" id="junbi"></a>

Microsoft Entra 관리 센터에서 Microsoft에서 제공하는 SAML 인증을 위한 XML 데이터를 다운로드합니다.\
자세한 내용은 [Microsoft Entra ID와 SSO를 연결하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function12002) 의 Microsoft Entra 관리 센터에서 SSO 연결 준비를 참조하십시오.

#### DirectCloud에서 Microsoft Entra ID와 협력

DirectCloud에서 Microsoft Entra ID와 함께 작동하도록 설정합니다.

1. [DirectCloud 관리 페이지](https://boxmanager.directcloud.jp/) 에서 사용자 > SSO 연동 메뉴를 선택하고 SAML 탭을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xG6b)

2. 「SAML2.0 연계」의 「사용한다」를 체크합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xG9p)

3. IdP 설정에서 Microsoft Entra ID 그룹 연결을 선택합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xGEf)

4. 화면을 아래로 스크롤하여 SAML 인증서 설정을 표시한 다음 파일 선택 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004dCLZ)

5. [Microsoft Entra 관리 센터에서 SSO 연결 준비를](https://help.directcloud.jp/s/article/operation-of-administrator-function12004#junbi) 위해 저장한 XML 파일을 선택합니다.
6. 다음 설정을 지정하고 저장 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMBB000000slfl)

| 품목        | 설명                                                                                                                                                                                                                       |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 로그인 계정    | <p>SSO 연결되지 않은 사용자가 로그인을 허용할지 여부를 설정합니다.</p><ul><li>IdP 계정만 사용<br>IdP 사용자만 사용할 수 있으며 사용자 > 사용자 관리 메뉴에 등록된 사용자는 사용할 수 없습니다.</li><li>IdP 및 DirectCloud 계정 모두 사용 IdP<br>사용자와 사용자 > 사용자 관리 메뉴에 등록된 사용자가 모두 활성화됩니다.</li></ul> |
| 로그아웃 시 처리 | <p>사용자 페이지에서 로그아웃할 때 IdP에서 로그아웃할지 여부를 설정합니다.</p><ul><li>DirectCloud만 로그아웃<br>IdP에서 로그아웃되지 않습니다.</li><li>DirectCloud와 IdP 모두에서 로그아웃<br>IdP에서도 연동하여 로그아웃됩니다.</li></ul>                                                     |
| 용량        | <p>IdP 사용자에게 할당할 내 상자의 용량을 계약 계획의 총 스토리지 용량 범위 내에서 설정합니다.<br>공유 폴더의 용량은 포함되지 않습니다.</p><ul><li>사용 가능한 문자: 1개 이상의 반각 숫자(단위: MB)</li><li>1024MB는 1GB로 변환됩니다.</li></ul>                                                      |

7. 상태에 유효( _고유 테넌트 ID_ )가 표시되는지 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xD0i)

#### DirectCloud에서 Microsoft Entra ID 그룹 정보 및 사용자 목록 얻기

DirectCloud에서 Microsoft Entra ID 그룹 정보 및 사용자 목록을 얻으려면 요청한 액세스를 허용하려면 Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자로 로그인해야 합니다.

1. 화면을 아래로 스크롤하고 사용자 그룹 정보 가져오기 설정에서 로그인 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMBB000000sl9v)

Microsoft Entra ID에 로그인하거나 사용 권한 상태에 따라 다음 단계 중 하나를 따르십시오.❶ Microsoft Entra ID에 로그인하지 않은 경우 계정 선택 화면이 표시됩니다. 2단계로 진행합니다.❷ "관리자 승인 필요"라는 화면이 나타나면 Microsoft Entra 관리 센터에서 관리자 역할이 할당되지 않은 사용자로 로그인한 것입니다. 이 경우 "관리자 계정이있는 경우 해당 계정으로 로그인합니다."를 클릭하면 "계정 선택"화면이 나타납니다. 2단계로 진행합니다.❸  Microsoft Entra ID에 Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자로 로그인했으며 요청한 액세스 권한이 부여된 경우 인증이나 권한 설정이 필요하지 않습니다. 4단계로 진행합니다.❹  Microsoft Entra ID에 Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자로 로그인했으며 요청한 액세스 권한이 없는 경우 요청된 권한 화면이 표시됩니다. . 3단계로 진행합니다.

2. Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자를 클릭하고 인증을 받고 로그인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMBB000000slgK)

요청한 액세스가 허용되지 않으면 요청된 권한 화면이 표시됩니다.

3. 조직 대리인으로 동의함을 선택하고 수락 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMBB000000slgU)

4. 사용자 그룹 정보 가져오기 설정에서 사용자 정보의 전자 메일 주소로 가져올 Microsoft Entra ID의 사용자 특성으로 UPN 또는 전자 메일을 선택합니다.\
   Microsoft Entra ID에 전자 메일 정보가 등록되지 않은 사용자의 경우 전자 메일을 선택한 경우에도 UPN이 등록됩니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xG0A)

5. 검색할 그룹을 설정하고 \[로드] 버튼을 클릭합니다.\
   Microsoft Entra 관리 센터에서 관리되는 그룹에 보안 그룹, Microsoft 365 그룹, 메일 사용 가능 보안 그룹, 메일 그룹 중 하나가 설정되어 있으면 DirectCloud에 그룹이 채워집니다. .

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xGRZ)

| 품목               | 설명                                                                                                                                                          |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 보안 그룹            | SharePoint와 같은 리소스를 활용하는 데 사용됩니다.                                                                                                                           |
| Microsoft 365 그룹 | 내부 및 외부에서 공동 작업을 수행하기 위해 SharePoint, Microsoft Teams 등에서 사용됩니다.                                                                                             |
| 메일 사용이 가능한 보안 그룹 | <p>SharePoint와 같은 리소스를 활용하는 데 사용됩니다. 그룹 구성원에게 메시지를 배포하는 기능이 있습니다.<br>Microsoft Entra 관리 센터가 아닌 Exchange 관리 센터 또는 Exchange 관리 셸에서 만들고, 수정하고, 삭제할 수 있습니다.</p> |
| 메일 그룹            | <p>그룹의 구성원에게 메시지를 배포하는 데 사용됩니다.<br>Microsoft Entra 관리 센터가 아닌 Exchange 관리 센터 또는 Exchange 관리 셸에서 만들고, 수정하고, 삭제할 수 있습니다.</p>                                   |

6. 3분 정도 경과한 후 페이지를 업데이트하여 '동작 중'이 표시되는지 확인합니다.\
   여기에서 최근 업데이트 날짜와 시간과 추가된 횟수를 확인할 수도 있습니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xGUn)

#### 연결된 Microsoft Entra ID 그룹 및 사용자 확인

1. 사용자 > 사용자 관리 메뉴를 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001x7cq)

2. '사용자 정보 관리' 아래에 'DirectCloud'와 'Microsoft Entra ID'라는 두 개의 탭이 만들어져 있는지 확인합니다.\
   또한 Microsoft Entra ID와 연결된 사용자의 ID에 표시가 표시되는지 ![azure.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMBB000000slYz) 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xGg5)

**DirectCloud 탭**

DirectCloud 탭에는 Microsoft Entra ID와 연동하기 전에 사용자 관리 화면과 동일한 내용이 표시됩니다.\
캡처된 사용자의 정보를 변경하거나 삭제하려면 Microsoft Entra ID 탭이 아닌 DirectCloud 탭에서 수행해야 합니다.\
"사용자 그룹 정보 가져오기" 설정에서 함께 작동하는 UPN 또는 이메일 주소는 사용자의 "이메일 주소"에 반영됩니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xGWQ)

**Microsoft Entra ID 탭**

Microsoft Entra ID 탭에는 다음 그룹 이름이 계층 구조로 표시됩니다.\
이 Microsoft Entra ID 탭에서는 캡처된 사용자의 등록 정보를 변경하거나 삭제할 수 없습니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001pOf\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001xGmX)

| 그룹 이름                    | 설명                                                                                                                                                                                                                                                                                                   |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 회 사 명                    | 클릭하면 계약하는 임차인에 등록된 모든 사용자가 표시됩니다.                                                                                                                                                                                                                                                                    |
| AzureADRoot              | <p>Microsoft Entra ID와 연동할 때 생성되는 첫 번째 계층의 폴더입니다. 이름을 바꿀 수 없습니다.<br>이 그룹 바로 아래에는 사용자가 등록되지 않습니다.</p>                                                                                                                                                                                                 |
| Microsoft Entra ID 그룹 이름 | <p>Microsoft Entra ID에서 가져온 그룹을 표시합니다.<br>그룹 이름을 클릭하면 Microsoft Entra ID로 해당 그룹에 속한 사용자를 볼 수 있습니다.</p><ul><li>캡처된 그룹은 상위 "AzureADRoot" 그룹 바로 아래에 병렬로 표시됩니다. Microsoft Entra ID에 등록된 그룹의 계층 구조는 반영되지 않습니다.</li><li>AzureADRoot 바로 아래에 만들 수 있는 그룹 수의 상한은 3,844입니다. 상한을 초과하면 정상적으로 캡처되지 않습니다.</li></ul> |
