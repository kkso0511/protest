---
description: '#드라이브 #설치'
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/quickstart/d_setup
---

# DirectCloud 드라이브 프로그램 설치 방법 테스트

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud 제품 페이지에서 DirectCloud 드라이브를 다운로드하고 설치하는 방법에 대해 설명합니다. 테스트

***

### 동작조건

* 처음으로 Windows에 DirectCloud 드라이브를 설치하는 경우에는, 반드시 관리자 권한으로 설치해야 합니다.
* 같은 PC에서 다른 Windows 사용자가 DirectCloud 드라이브를 사용하고 있는 경우, DirectCloud 드라이브를 설치할 때의 동작은 아래와 같습니다.
  *   Windows의 관리자 권한을 가진 사용자가 설치를 실행한 경우

      | DirectCloud 드라이브의 종류           | 동작                                                                                                                                                                 |
      | ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
      | <p>일반 버전<br>(32bit, 64bit)</p> | <p>다른 사용자가 DirectCloud 드라이브를 사용 중입니다. DirectCloud 드라이브를 강제 종료한 후 설치해도 되겠습니까?라는 화면이 표시됩니다.<br>'확인 버튼'을 클릭하면, 다른 사용자가 사용 중인 DirectCloud 드라이브가 강제 종료되고 설치가 실행됩니다.</p> |
  *   Windows의 관리자 권한을 보유하지 않은 사용자가 설치를 실행한 경우

      | DirectCloud 드라이브의 종류           | 동작                                                                                                          |
      | ------------------------------ | ----------------------------------------------------------------------------------------------------------- |
      | <p>일반 버전<br>(32bit, 64bit)</p> | <p>관리자의 비밀번호 입력 화면이 표시됩니다.<br>비밀번호를 입력하고 '확인'을 클릭하면, 다른 사용자가 사용 중인 DirectCloud 드라이브가 강제 종료되고 설치가 실행됩니다.</p> |
* 32bit 버전이 설치된 상태에서 64bit 버전의 인스톨러를 실행하면, '설치할 수 없습니다'라는 메시지가 표시되며 설치가 강제 종료됩니다.\
  이 경우에는 32bit 버전을 언인스톨한 후, 64bit 버전을 설치해 주십시오.
* IT 자산 관리 도구의 배포 기능을 이용하여 DirectCloud 드라이브의 사일런트 인스톨러를 배포하면, Windows 관리자 권한이 없는 사용자의 단말에도 DirectCloud 드라이브를 설치할 수 있습니다.
* 일반 DirectCloud 드라이브를 언인스톨하지 않은 상태에서 사일런트 설치 버전을 설치하면, 자동 업데이트 기능이 남아 있을 가능성이 있습니다.\
  반드시 현재의 DirectCloud 드라이브를 언인스톨하고 PC를 재시작한 후, 사일런트 설치 버전을 설치해 주십시오.
* 멀티 계정 모드의 제약 사항에 대하여\
  같은 Windows에 로그인한 여러 사용자가 DirectCloud 드라이브에 접근하여, 다른 사용자의 영향을 받지 않는 독립적인 환경에서 DirectCloud 드라이브를 이용할 수 있도록 하려면, DirectCloud 드라이브 설치 시 '어플리케이션 모드'에서 '멀티 계정 모드'를 선택해야 합니다.\
  멀티 계정 모드에서는 '사용자 권한'으로 드라이브 문자가 할당되지만, Windows에서는 기본적으로 관리자 권한으로 드라이브 문자를 할당하는 것이 권장되기 때문에, 아래와 같은 제약이 발생합니다.
* '관리자 권한'으로 DirectCloud 드라이브를 실행하는 경우\
  '멀티 계정 모드'에서는 '사용자 권한'으로 드라이브가 마운트됩니다.\
  DirectCloud 드라이브의 어플리케이션은 '사용자 권한'으로 실행되어야 하기 때문에, 프로그램의 메뉴 등에서 '관리자 권한으로 실행'을 선택하여 DirectCloud 드라이브를 실행하면, 권한 불일치(권한 충돌)로 인해 드라이브가 정상적으로 마운트되지 않습니다.
* '관리자 권한'으로 실행되는 프로그램에서 DirectCloud 드라이브에 접근하는 경우\
  Windows의 프로그램은 일반적으로 '사용자 권한'으로 실행되지만, 일부 프로그램은 '관리자 권한'이 필요합니다.\
  '관리자 권한'으로 실행되는 프로그램은, '사용자 권한'으로 마운트된 DirectCloud 드라이브에 접근할 때, 권한 불일치(권한 충돌)로 인해 파일에 정상적으로 접근하지 못할 가능성이 있습니다.
* '관리자 권한'이 필요한 폴더로 이동 또는 복사하는 경우\
  '사용자 권한'으로 할당된 DirectCloud 드라이브의 파일 또는 폴더를, '관리자 권한'이 필요한 폴더(C 드라이브 등)로 이동 또는 복사하면, 권한 불일치(권한 충돌)로 오류가 발생합니다.
*   설치하는 Windows용 DirectCloud 드라이브의 버전에 따라, '.Net Framework'와 'Microsoft Edge WebView2 Runtime'이 필요할 수 있습니다.\
    추가 설치가 필요한지 여부는 OS에 따라 다릅니다.

    * Windows 10／11\
      기본으로 설치되어 있으므로, 추가 설치가 필요하지 않습니다.
    * Windows Server 2019／2022\
      '.Net Framework'는 기본으로 설치되어 있으나, 'Microsoft Edge WebView2 Runtime'은 설치되어 있지 않습니다.
    * Windows Server 2016\
      '.Net Framework'와 'Microsoft Edge WebView2 Runtime' 모두 기본으로 설치되어 있지 않습니다.

    'Microsoft Edge WebView2 Runtime'은 Microsoft Office를 설치할 때 자동으로 설치되므로, 환경에 따라서는 추가 설치가 필요하지 않은 경우도 있습니다.\
    추가 설치가 필요한 경우에는, DirectCloud 드라이브 설치 시 자동으로 설치됩니다.\
    이로 인해 일반적인 설치보다 시간이 더 소요될 수 있습니다.\
    '.Net Framework 4.8' 및 'Microsoft Edge WebView2 Runtime'의 추가 설치를 위해서는, 인터넷에 연결 가능한 환경이 필요합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* [사용자가 이용할 수 있는 애플리케이션을 제한하는 방법](https://help.directcloud.net/admin_manual/security_policy/app_restrictions)에서 'DirectCloud 드라이브'가 허용되어 있지 않은 경우에는, DirectCloud 드라이브에 로그인할 수 없습니다.
* DirectCloud 드라이브에서 가능한 조작에 대해서는, [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/d_permission)을 참조해 주십시오.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**설치 프로그램 다운로드**
{% endhint %}

1. Web 브라우저에서 다이렉트클라우드  프로그램 [다운로드 ](https://www.directcloud.net/ko/downloads.php)페이지로 이동합니다.

<figure><img src="../../.gitbook/assets/image (1212).png" alt=""><figcaption></figcaption></figure>



2. 윈도우탐색기의 Windows 또는 Mac 아이콘을 클릭하여 프로그램을 다운로드합니다.



{% hint style="warning" %}
**Windows에서 설치 프로그램 실행**
{% endhint %}

1. 다운로드한 설치 프로그램 파일을 두 번 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.\
   사용자 계정 제어 화면이 표시되면 예를 클릭하여 DirectCloud 드라이브 설정 화면을 표시할 수 있습니다.



2. 다음 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1213).png" alt=""><figcaption></figcaption></figure>



3. DirectCloud 드라이브의 애플리케이션 모드를 선택하고 설치 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1214).png" alt=""><figcaption></figcaption></figure>

| 설치 버전 선택           | 설명                                                                                                                                                                         |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 일반 설치 (권장)         | <p>한 명의 사용자가 Windows에 로그인하여 DirectCloud 드라이브를 사용하려면 선택합니다.<br>DirectCloud 드라이브는 관리자 권한으로 실행됩니다.</p>                                                                        |
| Windows 멀티 사용자용 설치 | <p>동일한 Windows에 로그인한 여러 사용자가 DirectCloud 드라이브를 사용하려면 선택합니다.<br>DirectCloud 드라이브는 사용자 권한으로 실행됩니다.<br>다중 계정 모드의 제한 사항은 DirectCloud 드라이브를 설치하는 방법 [사양] 의 "작동 조건"을 참조하십시오.</p> |

응용 프로그램 설치가 시작됩니다.\
설치가 완료되면 DirectCloud 드라이브 설치 완료 화면이 나타납니다.



4. 지금 재부팅 또는 나중에 수동으로 재부팅을 선택하고 마침 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1215).png" alt=""><figcaption></figcaption></figure>

"지금 재부팅하겠습니다." 를 선택하면 즉시 컴퓨터가 다시 시작됩니다.\
"나중에 재부팅 하겠습니다. " 를  선택한 경우 사용자는 언제든지 컴퓨터를 다시 시작하여 DirectCloud 드라이브를 사용할 수 있습니다.



5. 다시 시작한 후 바탕화면에  바로가기  아이콘이 생성 되어있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1216).png" alt=""><figcaption></figcaption></figure>
