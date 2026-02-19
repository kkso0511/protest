---
metaLinks:
  alternates:
    - https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/sso/sso
---

# SSO 연계에 관한 사양 및 주의사항

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는, IdP와 SSO 연동함으로써, IdP가 제공하는 인증 정보를 이용해서 DirectCloud에 싱글 사인온할 수 있습니다.\
이 매뉴얼 에서는, DirectCloud의 Web 매뉴얼에 기재되어 있는 SSO 연동에 관한 용어의 정의, 및 DirectCloud와 IdP와의 연동에 있어서의 사양, SAML 연동 시의 주의사항 등에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* IdP가 제공하는 서비스, 사용자 인터페이스(UI), 명칭 등은 예고 없이 변경될 수 있습니다.\
  이에 따라 DirectCloud의 Web 매뉴얼에서 사용하고 있는 화면 명칭 등도 변경될 수 있습니다.\
  이 경우에는 제공되는 서비스, 기능, UI 등에 맞추어 본 매뉴얼을 진행해 주십시오.

***

### 설명 <a href="#a05" id="a05"></a>

본 매뉴얼에서는, 아래 항목에 대해 설명하고 있습니다.

* SSO 관련 용어
* DirectCloud에서 동작하는 IdP에 대해
* 유저 정보의 연동과 갱신에 대해
* 액세스 제어에 대해
* 로그인과 로그아웃에 대해
* Open API의 이용에 대해



{% hint style="warning" %}
**SSO 관련 용어**
{% endhint %}

* **SSO(Single Sign-On, 싱글 사인온)**\
  한 번 사용자 ID와 비밀번호로 인증하면, 서로 다른 서비스나 시스템 등을 이용할 수 있도록 하는 구조를 의미합니다. \
  DirectCloud에서는 LDAP와 SAML을 통해 싱글 사인온을 수행하는 기능을 제공하고 있습니다.\
  SSO와 관련된 문서 등에서는 인증 정보를 연동하는 것을, 제공되는 서비스나 프로토콜에 따라 SSO 연동, SAML 연동, ID 연동 등 여러 용어로 부르는 경우가 있습니다.\
  본 매뉴얼에서는 프로토콜에 대해 설명하는 경우를 제외하고, 기본적으로 'SSO 연동'이라는 용어를 사용하고 있습니다.
* **IdP(Identity Provider, Identity Provider)**\
  SSO에서 사용되는 인증 정보를 제공하는 공급자를 의미합니다.\
  IdP 인증에서는 SAML이나 OpenID 등의 프로토콜이 사용됩니다.\
  DirectCloud에서는 SAML을 사용한 인증을 수행합니다.
* **SP(Service Provider, 서비스 프로바이더)**\
  SSO에서 사용자가 로그인하는 애플리케이션을 의미합니다.\
  SP 사용자는 SP와 연동된 IdP에서 인증을 수행한 후, SP에 로그인합니다.\
  DirectCloud도 SP에 해당하지만, 본 매뉴얼에서는 SP라는 용어를 사용하지 않고 DirectCloud로 표기합니다.
* **SAML (Security Assertion Markup Language)**\
  IdP와 SP 간에 사용자 인증과 정보를 공유하기 위해 사용되는 XML 기반의 표준 규격을 의미합니다.\
  최신 버전은 SAML 2.0입니다.\
  SAML에는 사용자의 인증 정보 외에도, 속성 정보나 사용자에 대한 권한 부여 등의 정보를 기재할 수 있습니다.\
  SAML을 사용하여 IdP와 인증을 수행하고, IdP의 인증 정보를 취득하는 것을 'SAML 인증'이라고 합니다.
* **SAML 연동**\
  SAML을 사용하여 IdP와 연동하고, 사용자 정보를 사용할 수 있도록 하는 것을 의미합니다.
* **ID 연계**\
  IdP와 SP에서 사용자 ID를 매핑하는 것을 의미합니다.
* **JIT(Just In Time, 저스트 인 타임) 프로비저닝**\
  SAML을 통해 사용자가 처음으로 DirectCloud에 SSO 로그인할 때, DirectCloud에 사용자 계정이 자동으로 생성되는 구조를 의미합니다.
* **LDAP(Lightweight Directory Access Protocol)**\
  네트워크에서 리소스를 관리하기 위한 디렉터리 서비스에서 사용되는 프로토콜입니다.\
  부서 및 이메일 주소와 같은 속성 정보를 포함하는 사용자 정보, 파일, 장치 등의 정보를 중앙에서 관리하기 위해 기업 내 네트워크 등에서 사용됩니다.\
  사용자는 LDAP 자격 증명을 사용하여 싱글 사인온하여 기업 내 서비스 등을 이용할 수 있습니다.



{% hint style="warning" %}
**DirectCloud에서 동작하는 IdP에 대해**
{% endhint %}

**\[여러 IdP와의 연계에 관한 주의사항]**

여러 IdP와 동시에 SSO 연동하는 것은 불가능합니다.



**\[DirectCloud에서 사용할 수 있는 IdP]**

Microsoft Entra ID\
Microsoft Entra ID 그룹 연동\
ADFS\
CloudGate UNO\
Google Workspace\
OneLogin\
Sateraito Office / NextSet\
HENNGE One\
Salesforce\
Okta\
IIJ ID 서비스\
TrustLogin\
OPTiM ID+\
Soliton OneGate\
Qualitia CLOUD\
PassLogic\
ID Entrance



{% hint style="warning" %}
**유저 정보의 연동과 갱신에 대해**
{% endhint %}

**\[사용자 정보 연동에 관한 제한 사항]**

* SSO 연동의 사용자 수에는 제한이 없습니다.
* 연동되는 IdP 사용자의 속성과 동일한 문자열이 DirectCloud의 사용자 ID로 설정되어 있는 경우, SSO 연동으로 DirectCloud에 로그인하더라도 '이름', '소속 그룹', '기능 제한', '접근 제어' 등의 정보는 변경되지 않습니다. 또한 부여되어 있던 접근 권한도 삭제되지 않습니다. 사용자 ID에는 IdP 아이콘만 추가됩니다.
* IdP에서 사용자가 삭제되더라도, DirectCloud에서 연동되어 있는 사용자 ID는 삭제되거나 비활성화되지 않습니다.\
  DirectCloud에서는 Guest ID로 사용 중인 이메일 주소와 동일한 사용자 ID를 등록할 수 없습니다. 이 경우 Guest를 삭제하면 사용자를 등록할 수 있게 됩니다.



**\[SSO 연동에서 사용되는 이메일 주소 형식의 사용자 ID에 대해]**

DirectCloud의 SSO 연동에서는 이메일 주소 형식(사용자명@도메인)의 사용자 ID가 사용됩니다.\
'계정 관리' > '사용자' 메뉴에 등록되어 있지 않은 사용자가 처음으로 SSO 로그인했을 때, 또는 '사용자 목록 가져오기' 기능을 통해 사용자 정보가 취득되었을 때, 이메일 주소 형식의 사용자 ID로 사용자가 등록됩니다.\
사전에 DirectCloud의 사용자 ID를 이메일 주소 형식으로 생성해 두면, SSO 연동 시 IdP의 정보를 연결할 수 있습니다.



**\[사용자 정보 업데이트에 관한 주의 사항]**

* SSO 연동된 사용자 및 '사용자 목록 가져오기' 기능으로 취득된 사용자에게는, '계정관리' > '사용자' 메뉴의 '사용자 ID' 앞에 연동된 IdP의 아이콘이 표시됩니다.
* 사용자 정보의 자동 업데이트는 지원하지 않습니다.
  * JIT 프로비저닝으로 SSO 로그인하는 경우:\
    연동된 IdP 측의 사용자 정보가 변경되더라도, IdP 사용자가 DirectCloud에 SSO 로그인할 때 DirectCloud의 기존 사용자 정보는 업데이트되지 않습니다.
  *   '사용자 목록 가져오기'로 1시간마다 자동으로 사용자 목록을 가져올 수 있는 IdP의 경우:\
      IdP에 새로 추가된 사용자가 있는 경우에는 1시간마다 DirectCloud에 반영되지만, 한 번 추가된 사용자의 정보가 IdP 측에서 업데이트되더라도 DirectCloud에는 반영되지 않습니다.\
      연동을 해제할 때까지 사용자 정보는 1시간마다 동기화됩니다.

      (**NOTE**:  단, Microsoft Entra ID의 '사용자 목록 가져오기' 및 '사용자·그룹 정보 가져오기'로 사용자 목록을 가져오는 경우에만 '이름'과 '메일 주소'가 업데이트됩니다.)
  * '사용자 목록 가져오기'에서 CSV 파일을 사용하여 사용자 목록을 업데이트하는 IdP의 경우:\
    수동으로 사용자 정보를 업데이트할 수 있습니다.\
    IdP에 새로 사용자가 추가되더라도, DirectCloud에는 자동으로 반영되지 않습니다.
* SSO 연동 후에 '계정관리' > '사용자' 메뉴에서 IdP와 연동된 사용자 정보의 '이름'을 변경한 경우, IdP 측에 등록된 사용자 정보와 차이가 발생할 수 있습니다.
* DirectCloud의 '사용자 목록 가져오기' 기능을 지원하는 IdP의 경우, IdP의 사용자 정보 '가져오기'를 실행한 시점에 사용자 정보가 반영됩니다.



**\[IdP 속성과 DirectCloud 사용자 정보 간의 대비]**

아래 표에는 개별 사용자가 DirectCloud에 처음 로그인했을 때 사용자 계정이 생성되는 경우의 사양에 대해 기재되어 있습니다.\
사용자 일괄 가져오기를 지원하는 IdP의 경우에는, 사용자를 일괄로 가져올 때 아래 표와는 다른 속성이 연결될 수 있다는 점에 유의해 주십시오.

<table><thead><tr><th></th><th>IdP 속성</th><th>IdP 속성</th><th width="116.5">DC 사용자 정보</th><th width="97">DC 사용자 정보</th><th width="90">DC 사용자 정보</th></tr></thead><tbody><tr><td> </td><td>관리 화면 표시</td><td>유저 연동 작업 시</td><td>사용자 ID</td><td>이름</td><td>이메일 주소</td></tr><tr><td>Microsoft Entra ID</td><td>이름</td><td>-</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>이메일 주소</td><td>-</td><td> ◯</td><td></td><td>◯</td></tr><tr><td>ADFS</td><td>표시 이름</td><td>displayname</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>UserPrincipalName</td><td>upn</td><td>◯</td><td></td><td></td></tr><tr><td></td><td>이메일 주소</td><td>emailaddress</td><td></td><td></td><td>◯</td></tr><tr><td>CloudGate UNO</td><td>표시 이름</td><td>GivenName + SurName</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>사용자 ID</td><td>EmailAddress</td><td> ◯</td><td></td><td>◯</td></tr><tr><td>Google Workspace</td><td>이름</td><td>firstname + lastname</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>이메일 주소</td><td>Email</td><td>◯ </td><td></td><td>◯</td></tr><tr><td>OneLogin</td><td>성 + 이름</td><td>lastname + firstname</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>이메일 주소</td><td>Email</td><td>◯</td><td></td><td>◯</td></tr><tr><td>Sateraito Office / NextSet</td><td>성 + 이름</td><td>lastname + firstname</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>이메일 주소</td><td>email</td><td>◯</td><td></td><td>◯</td></tr><tr><td>HENNGE One</td><td>표시 이름</td><td>{user.display_name}</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>UserPrincipalName</td><td>{user.upn}</td><td>◯</td><td> </td><td></td></tr><tr><td></td><td>이메일 주소</td><td> {user.email}</td><td> </td><td></td><td>◯</td></tr><tr><td>Salesforce</td><td>성명</td><td>username</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>사용자 이름</td><td>userId</td><td>◯</td><td></td><td></td></tr><tr><td></td><td>이메일 주소</td><td>email</td><td></td><td></td><td></td></tr><tr><td>Okta</td><td>성 + 이름</td><td>user.firstName + user.lastName</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>이메일 주소<br>또는<br>사용자 이름</td><td>user.email<br>또는<br>user.login</td><td>◯</td><td></td><td>◯</td></tr><tr><td>TrustLogin</td><td>이름</td><td>멤버 성 + 멤버 이름</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>회원 이메일 주소</td><td>회원 이메일 주소</td><td>◯</td><td></td><td>◯</td></tr><tr><td>OPTiM ID+</td><td>이름</td><td>이름</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>이메일 주소</td><td>이메일 주소</td><td>◯</td><td></td><td>◯</td></tr><tr><td>IIJ ID 서비스</td><td>성명</td><td>성 + 이름</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>ID</td><td>알림 대상 이메일 주소</td><td>◯</td><td></td><td>◯</td></tr><tr><td>Soliton OneGate</td><td>로그인 이름</td><td>id</td><td>◯</td><td> </td><td> </td></tr><tr><td></td><td>SSO User</td><td>NameID</td><td></td><td> ◯</td><td></td></tr><tr><td></td><td>이메일 주소</td><td>email</td><td> </td><td></td><td>◯</td></tr><tr><td>Qualitia CLOUD</td><td>로그인 ID</td><td>LOGIN_ID</td><td> </td><td> </td><td> </td></tr><tr><td></td><td>이름</td><td>NAME</td><td> </td><td> </td><td></td></tr><tr><td></td><td>이메일 주소</td><td>EXTERNAL_ID</td><td>◯</td><td>◯</td><td>◯</td></tr><tr><td>PassLogic</td><td>성명</td><td>성명</td><td> </td><td>◯</td><td> </td></tr><tr><td></td><td>이메일 주소</td><td>이메일 주소</td><td>◯</td><td></td><td>◯</td></tr><tr><td>ID Entrance</td><td>사용자 이름</td><td>username</td><td>◯</td><td>◯</td><td>◯</td></tr><tr><td></td><td>이메일 주소</td><td>-</td><td>◯</td><td></td><td>◯</td></tr></tbody></table>



**\[IdP의 일부 사용자를 얻는 방법]**

DirectCloud와 IdP 간의 SSO 연동에서는 일부 사용자를 선택하고 검색할 수 없습니다.\
그러나 Microsoft Entra ID의 경우 Microsoft Entra 관리 센터의 "응용 프로그램" > "엔터프라이즈 응용 프로그램"의 응용 프로그램 중 다음 두 가지 모두에 해당하는 응용 프로그램의 "사용자 및 그룹"에 등록 된 사용자를 얻을 수 있습니다. 합니다.

* SSO 연동 또는 SSO 그룹 연동 시 생성된 'DirectCloud' 애플리케이션
* 현재 로그인한 회사 ID에 연결되어 있는 애플리케이션

자세한 내용은 [Microsoft Entra ID 사용자 목록을 가져오는 방법을](https://help.directcloud.jp/s/article/operation-of-administrator-function12003) 참조하십시오.



**IdP 그룹을 얻는 방법**

DirectCloud와 IdP 간의 SSO 연동에서는 그룹을 연동할 수 없습니다.\
그러나 Microsoft Entra ID의 경우 Microsoft Entra ID의 그룹 유형을 선택하여 특정 그룹을 가져올 수 있습니다.\
자세한 내용은 [Microsoft Entra ID 그룹 정보를 가져오는 방법을](https://help.directcloud.jp/s/article/operation-of-administrator-function12004) 참조하십시오.



**사용자 정보 업데이트에 대한 참고 사항**

* SSO 연동 후 IdP 관리 화면에서 사용자 정보를 업데이트하면 해당 사용자로 DirectCloud에 로그인해도 사용자 정보가 업데이트되지 않습니다.
* SSO 연동 후, "사용자" > "사용자 관리"메뉴에서 IdP와 연동하는 사용자 정보의 "이름"을 변경하면 IdP 측에 등록된 사용자 정보와의 차이가 발생합니다.
* DirectCloud의 「사용자 일람」기능에 대응하고 있는 IdP의 경우, IdP의 유저 정보의 「캡처」를 실행한 타이밍에, 유저 정보가 캡쳐됩니다.
* 「유저 일람」을 취득한 뒤의, 유저 정보의 자동 갱신에는 대응하고 있지 않습니다.\
  새로 추가된 사용자가 있는 경우 1시간마다 반영되지만 기존 사용자로 로그인해도 사용자 정보는 업데이트되지 않습니다.\
  연결이 해제될 때까지 사용자 정보는 매시간 동기화됩니다.



**사용자 목록 캡처 기능을 지원하는 IdP**

| IdP                        | 대응 |
| -------------------------- | -- |
| Microsoft Entra ID         | ◯  |
| ADFS                       |    |
| CloudGate UNO              |    |
| Google Workspace           |    |
| OneLogin                   |    |
| Sateraito Office / NextSet | ◯  |
| HENNGE One                 | ◯  |
| Salesforce                 | ◯  |
| Okta                       | ◯  |
| TrustLogin                 |    |
| OPTiM ID+                  | ◯  |
| IIJ ID 서비스                 | ◯  |
| Soliton OneGate            |    |
| Qualitia CLOUD             |    |
| PassLogic                  |    |
| ID Entrance                |    |



**용량 설정이 적용되는 사용자**

관리 페이지 사용자 > SSO 연합 메뉴의 SAML 탭에서 용량에 지정한 숫자는 새로 사용자를 작성할 때만 사용자 정보에 적용됩니다.\
연동한 후, 사용자 별 용량을 일괄 변경하는 경우는, [사용자 정보를 일괄로 변경하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11089) 의 순서로, CSV 파일을 이용해 정보를 변경해 주세요.



**검색된 사용자를 사용 중지하는 방법**

다음 단계를 통해 획득한 사용자를 사용 중지할 수 있습니다.

1. 사용자 > SSO 연동 메뉴의 SAML 탭에서 IdP에서 테넌트 전체 사용자 목록 가져오기
2. 사용자 > 사용자 관리 메뉴에서 SSO 연결이 필요하지 않은 사용자의 상태를 비활성화합니다.



**사용자 정보를 업데이트하는 방법**

"사용자 목록" 기능으로 사용자 정보를 동기화할 수 없는 IdP의 경우, SSO와 연동하는 사용자 정보는 다음 절차에 따라 변경할 수 있습니다.\
그러나 엔터프라이즈 플랜에서 DirectCloud 감사를 사용하는 경우 이 방법으로 사용자 정보를 변경할 수 없습니다. 자세한 내용은 [DirectCloud 감사가 활성화된 경우 참고 사항을](https://help.directcloud.jp/s/article/operation-of-administrator-function12001#audit_notes) 참조하십시오.

1. DirectCloud 관리 페이지에서 사용자 > 사용자 관리 메뉴를 표시하고 변경하려는 사용자 삭제
2. SSO와 협력하는 IdP의 관리 화면에서 사용자 정보 변경
3. 사용자 정보를 변경한 사용자로 DirectCloud에 싱글 사인온



**DirectCloud 감사가 활성화된 경우 주의사항**

계약 플랜이 엔터프라이즈 플랜이고 무료 옵션인 'DirectCloud 감사'가 사용 설정된 경우 삭제된 사용자의 ID를 다시 활성화할 수 없습니다. 또한 삭제된 사용자 ID로 사용자를 다시 추가할 수 없습니다.\
따라서 [사용자 정보를 업데이트하는 방식](https://help.directcloud.jp/s/article/operation-of-administrator-function12001#user_update) 으로 사용자를 삭제하면 해당 사용자 ID로 DirectCloud에 싱글 사인온할 수 없습니다.

#### 액세스 제어 정보 <a href="#s_04" id="s_04"></a>

**액세스 제어에 관한 주의사항**

* IdP 사용자에게는 DirectCloud '이중 인증'이 적용되지 않습니다.
* 장치 인증 및 IP 주소 제한은 다음 절차에 따라 IdP 사용자에게도 적용할 수 있습니다.

**IdP 사용자에게 기기 인증을 적용하는 방법**

1. 관리 페이지 보안 > 액세스 제어 메뉴에서 장치 관리 탭을 클릭합니다.
2. 장치 인증 설정에서 관리자 승인 필요를 선택합니다.
3. IdP 사용자 포함을 선택합니다.

자세한 내용은 [사용자가 로그인할 수 있는 장치를 제한하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11032) 에 대한 장치 인증 설정을 참조하십시오.

**IdP 사용자에게 IP 주소 제한을 적용하는 방법**

1. 관리 페이지 보안 > 액세스 제어 메뉴에서 IP 주소 제한 탭을 클릭합니다.
2. 사용자의 IP 주소 제한 설정에서 사용을 선택합니다.\
   설정은 즉시 저장됩니다.
3. 대상 드롭다운 목록에서 IdP 사용자 또는 모든 사용자를 선택합니다.\
   설정은 즉시 저장됩니다.

자세한 내용은 [사용자 페이지에 로그인할 수 있는 IP 주소를 제한하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11035) 을 참조하십시오.

#### 로그인 및 로그아웃 정보 <a href="#s_05" id="s_05"></a>

**DirectCloud에 로그인하기 위한 참고 사항**

* SSO 연동을 수행한 사용자 ID의 비밀번호 정보는 DirectCloud에 저장되지 않습니다. 따라서 SSO 연계 계정을 이용하여 관리 페이지의 로그인 화면에서 직접 로그인할 수 없습니다.\
  다음 방법 중 하나로 관리 페이지에 로그인합니다.
  * 사용자 페이지에 SSO로 로그인 한 후 화면 오른쪽 상단의 "관리 페이지로"버튼을 클릭하십시오.
  * SSO와 협력하지 않은 사용자를 만들고 관리 페이지에 직접 로그인
* 관리 페이지 사용자 > SSO 연동 메뉴의 SAML 탭에서 로그인 계정의 IdP 계정만 사용을 선택하면 DirectCloud 로컬 사용자 및 게스트 사용자로 로그인할 수 없습니다.

**자동으로 SSO 로그인하는 방법**

[사용자 로그인 페이지의 하위 도메인을 설정하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11161) 으로 로그인할 때 회사 ID 입력을 생략하여 로그인 화면에서 "SSO로 로그인"을 클릭한 후 자동으로 SSO 로그인하도록 설정할 수 있습니다.

**DirectCloud 드라이브 또는 PC 애플리케이션에서 SSO 로그인하는 방법**

PC 응용 프로그램 또는 DirectCloud 드라이브를 사용하여 SSO 로그인을 허용하도록 설정하는 경우 관리 페이지의 보안 > 액세스 제어 메뉴에서 해당 응용 프로그램을 선택합니다.

**모바일 애플리케이션에서 SSO 로그인하는 방법**

모바일 애플리케이션에서 웹 사용자 페이지에 액세스하여 SSO 로그인하면 '모바일 기기에서 사용하려면 전용 앱이 필요합니다.'라는 오류 메시지가 표시됩니다.\
iOS 및 Android 기기를 사용하여 로그인하는 경우 관리 페이지의 보안 > 액세스 제어 메뉴에서 해당 응용 프로그램을 선택하고 응용 프로그램을 통해 SSO 로그인하십시오.

**로그아웃 시 주의사항**

* 관리 페이지 사용자 > SSO 연동 메뉴의 로그아웃 시 처리 설정은 DirectCloud의 모든 애플리케이션에서 작동합니다.
* 로그아웃 시 처리 설정에서 DirectCloud와 IdP 모두에서 로그아웃을 선택할 수 있는 IdP는 다음과 같습니다.
  * Microsoft Entra ID
  * ADFS
  * OneLogin
* 관리 페이지 “사용자” > “SSO 연동” 메뉴에서 다음 IdP를 선택한 경우, “로그아웃 시 처리” 설정은 “DirectCloud만 로그아웃”으로 고정되고 “DirectCloud와 IdP 모두에서 로그아웃” 항목은 선택 할 수 없습니다.
  * CloudGate UNO
  * Google Workspace
  * Sateraito Office / NextSet
  * HENNGE One
  * Salesforce
  * Okta
  * IIJ ID 서비스
  * Trustlogin
  * OPTiM ID+
  * Soliton OneGate
  * Qualitia CLOUD
  * PassLogic
  * ID Entrance
* 다음과 같은 이유로 SSO 연동을 통한 로그인 세션이 종료된 경우 싱글 로그아웃이 적용되지 않습니다.
  * 동시 로그인 제한 설정
  * 자동 로그아웃 설정
  * 액세스 토큰 수명 만료
  * 서버 장애로 세션 종료
  * 업데이트 또는 유지 보수로 세션 종료

#### DirectCloud API 사용 정보 <a href="#s_06" id="s_06"></a>

**SSO 연동 사용자로 API를 사용하는 방법**

1. [API 참조를](https://directcloud.jp/api_reference/detail/%E3%83%A6%E3%83%BC%E3%82%B6%E3%83%BC/SSO) 표시합니다.
2. 다음 절차에 따라 액세스 토큰을 검색합니다.
   * 액세스 키 얻기
   * SSO 로그인 화면 표시
   * 자격 증명 조회
3. 매개변수에 액세스 토큰을 입력하고 요청 메소드의 GET 또는 POST로 HTTP 요청을 보냅니다.

**SSO가 작동하지 않는 사용자로 사용자 API를 사용하는 방법**

다음과 같은 방법으로 SSO가 작동하지 않는 사용자와 관리자를 만들어 DirectCloud API의 사용자 API를 활용할 수 있습니다.

1. SSO에서 사용자 페이지에 로그인하고 관리 페이지에 액세스합니다.
2. 사용자 > SSO 연합 메뉴를 선택하고 SAML 탭을 클릭합니다.
3. 로그인 계정 설정에서 IdP 및 DirectCloud 계정 모두 사용을 선택합니다.
4. [사용자를 추가하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11079) 의 단계에서 사용자를 추가합니다.
5. 4단계에서 추가한 사용자의 암호를 설정합니다.
6. 추가한 사용자의 사용자 ID와 비밀번호로 사용자 API를 사용합니다.

**SSO가 작동하지 않는 사용자로 관리자 API를 사용하는 방법**

다음과 같은 방법으로 SSO가 작동하지 않는 사용자에게 관리자 권한을 추가하여 DirectCloud API의 관리자 API를 활용할 수 있습니다.

1. [SSO가 연결되지 않은 사용자로 사용자 API를 사용하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function12001#use_userapi) 의 1\~5단계를 수행합니다.
2. [사용자에게 일반 관리자 권한을 추가하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11119) 의 단계에서 만든 사용자를 관리자로 설정합니다.
3. 관리자로 설정한 사용자의 사용자 ID와 비밀번호로 관리자 API를 사용합니다.
