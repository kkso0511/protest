---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/sso/microsoft-entra-id
---

# Microsoft Entra ID 사용자 목록을 가져오는 방법

### 개요 <a href="#a03" id="a03"></a>

Microsoft Entra ID를 사용하면 Office 365, Intune, Dynamics CRM Online과 같은 Microsoft 클라우드 서비스뿐만 아니라 다양한 클라우드 서비스를 안전하게 인증할 수 있습니다.\
이 절에서는 SSO에서 작동하는 Microsoft Entra ID에서 사용자 목록을 검색하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Microsoft 및 기타 회사에서 제공하는 서비스 및 사용자 인터페이스(UI) 등은 예고 없이 변경될 수 있습니다. 이에 따라 본 기사에서 사용하고 있는 화면의 명칭 등도 바뀔 가능성이 있습니다. 그 경우, 제공되고 있는 서비스나 기능, UI등에 맞추어, 이 기사를 실행하도록 해 주세요.
* Azure Active Directory의 이름은 2023년 10월 1일에 Microsoft Entra ID로 변경되었습니다.
* Microsoft Entra ID에 로그인하기 위한 MFA(다중 요소 인증)와 같은 인증 방법은 Microsoft Entra ID 설정에 따라 다릅니다. 절차를 시작하기 전에 확인해야 합니다.
* Microsoft Entra ID와의 연동은 매시간 동기화 처리를 수행하여 사용자 목록을 검색합니다. 동기화할 횟수나 시간을 변경할 수 없습니다.
* 일단 사용자 목록 검색이 설정되면 사용자 목록 검색에 실패하면 매 시간마다 재시도 처리가 수행됩니다. 첫 번째 재시도 처리가 실패하면 "사용자 목록 검색 실패 알림"이라는 제목의 알림 메일이 전송됩니다.
* 사용자 > 사용자 관리 메뉴에서 사용자의 상태를 사용 안함으로 변경하여 사용자별로 DirectCloud에 대한 로그인을 제한할 수 있습니다.
* SSO에서 작동하는 Microsoft Entra ID의 계정 상태가 '사용 안 함'인 경우 '사용자 목록 가져오기'는 DirectCloud에 사용자를 가져오지만 잘못된 계정으로 DirectCloud에 SSO 로그인할 수는 없습니다.
* UPN(User Principal Name, User Principal Name)은 Microsoft Active Directory 등에서 사용자 식별에 사용되는 'User Name@Domain Name' 형식의 로그인 이름입니다. Active Directory에서는 일반적으로 전자 메일 주소를 UPN으로 설정하지만 반드시 일치하는 것은 아닙니다.\
  DirectCloud에서는 사용자의 UPN이 이메일 주소와 일치하는지 확인할 수 없습니다.
* 이 문서의 단계에서 사용자 목록을 얻으면 사용자 > 사용자 관리 메뉴에 캡처된 사용자의 사용자 ID가 Microsoft Entra 관리 센터에서 관리되는 사용자의 사용자 주체 이름과 연결됩니다. .
* Microsoft Entra 관리 센터에서 관리하는 사용자의 속성에서 메일에 전자 메일 주소가 설정되어 있는 경우 사용자 주체 이름 외에도 해당 전자 메일 주소로 DirectCloud에 SSO 로그인할 수 있습니다. 합니다.\
  이 경우 처음 이메일 주소로 SSO 로그인했을 때 사용자 > 사용자 관리 메뉴에 이 문서의 단계에서 얻은 '#EXT#'이 포함된 사용자 주체 이름의 사용자 ID 외에 주소의 사용자 ID가 추가됩니다.\
  결과적으로 DirectCloud에는 두 개의 ID가 추가되지만 Microsoft Entra 관리 센터에서는 단일 사용자로 관리됩니다.
* Microsoft Entra 관리 센터에서 외부 사용자를 초대한 경우에는 속성의 메일에 외부 사용자의 이메일 주소가 설정됩니다.\
  DirectCloud에 SSO 로그인하는 경우 Microsoft 계정 선택 화면에서 이 이메일 주소를 지정해야 합니다.
* "사용자 목록 가져 오기"의 "대상"설정에서 "엔터프라이즈 응용 프로그램 사용자"를 선택하고 "가져 오기"버튼을 클릭하면 Microsoft Entra 관리 센터에서 연결된 응용 프로그램의 "사용자 및 그룹"에 등록됩니다. 중인 그룹에 속한 사용자는 DirectCloud에 포함되지 않습니다. '사용자 및 그룹' 바로 아래의 사용자만 캡처됩니다.
* Microsoft Entra ID의 사용자 목록을 얻으려면 Microsoft Entra 관리 센터에서 사용자, 그룹, 응용 프로그램을 관리하는 역할 및 디렉터리를 탐색하는 역할이 할당된 사용자로 Microsoft에 로그인하고 사용 권한을 수락합니다. 해야 합니다.\
  사용자, 그룹 및 애플리케이션을 관리할 수 있는 관리자 역할에는 "사용자 관리자", "그룹 관리자", "응용 프로그램 관리자"가 있습니다. 또한 "디렉토리 뷰어"의 역할도 필요합니다.\
  관리자 역할에 대한 자세한 내용은 Microsoft 설명서를 참조하십시오.

### 절차 <a href="#a05" id="a05"></a>

#### DirectCloud에서 Microsoft Entra ID의 사용자 목록 얻기

DirectCloud에서 Microsoft Entra ID의 사용자 목록을 가져오려면 요청한 액세스를 허용하려면 Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자로 로그인해야 합니다.

1. [Microsoft Entra ID와 SSO 연동 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function12002) 에 따라 Microsoft Entra ID와 SSO 연동을 사용하도록 설정합니다.
2. DirectCloud 관리 페이지에서 사용자 > SSO 연동 메뉴를 선택하고 SAML 탭을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001wm25)

3. 화면을 아래로 스크롤하고 '사용자 목록 가져오기' 설정의 '로그인' 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMBB000000skmt)

Microsoft Entra ID에 로그인하는 상황에 따라 다음 단계 중 하나를 따르십시오.❶ Microsoft Entra ID에 로그인하지 않은 경우 계정 선택 화면이 표시됩니다. 4단계로 진행합니다.❷ "관리자 승인 필요"라는 화면이 나타나면 Microsoft Entra 관리 센터에서 관리자 역할이 할당되지 않은 사용자로 로그인한 것입니다. 이 경우 "관리자 계정이있는 경우 해당 계정으로 로그인합니다."를 클릭하면 "계정 선택"화면이 나타납니다. 4단계로 진행합니다.❸ Microsoft Entra ID에 Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자로 로그인한 경우 요청된 사용 권한 화면이 표시됩니다. 5단계로 진행합니다.

4. Microsoft Entra 관리 센터에서 관리자 역할이 할당된 사용자를 클릭하고 인증을 받고 로그인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMBB000000skvs)

요청된 사용 권한 화면이 표시됩니다.

5. 조직 대리인으로 동의함을 선택하고 수락 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004yRz7)

6. 사용자 목록 가져오기의 대상 설정에서 DirectCloud로 가져올 사용자의 범위를 지정합니다.

* 모든 사용자:\
  Microsoft Entra 관리 센터의 "모든 사용자"에 등록된 사용자를 캡처합니다.
* 엔터프라이즈 응용 프로그램 사용자:\
  Microsoft Entra 관리 센터의 응용 프로그램 > 엔터프라이즈 응용 프로그램의 응용 프로그램 중 다음 두 가지 모두에 해당하는 응용 프로그램의 사용자 및 그룹에 등록된 사용자가 포함됩니다.
  * SSO 연동 또는 SSO 그룹 연동 시 생성된 'DirectCloud' 애플리케이션
  * 현재 로그인한 회사 ID에 연결되어 있는 애플리케이션

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMQ8000003zWin)

7. "사용자 목록 가져오기"의 "이메일 주소" 설정에서 사용자 정보의 "이메일 주소"로 가져올 Microsoft Entra ID의 사용자 특성으로 "UPN" 또는 "이메일"을 선택합니다.\
   Microsoft Entra ID에 전자 메일 정보가 등록되지 않은 사용자의 경우 전자 메일을 선택한 경우에도 UPN이 등록됩니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMQ8000003zWpF)

8. 로드 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMQ8000003zWNq)

9. 3분 정도 경과한 후 페이지를 업데이트하여 '동작 중'이 표시되는지 확인합니다.\
   여기에서 최근 업데이트 날짜와 시간과 추가된 횟수를 확인할 수도 있습니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMQ8000003zVra)

10. 사용자 > 사용자 관리 메뉴를 선택하여 사용자가 캡처되었는지 확인합니다.\
    Microsoft Entra ID와 연동된 사용자의 ID에는 ![azure.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMBB000000skuW) 표시가 표시됩니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002eqz\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001wm8X)
