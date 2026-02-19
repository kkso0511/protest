---
description: '#태그 #설치'
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/quickstart/directcloud-shield-irm-pc-drive
---

# DirectCloud-SHIELD IRM을 지원하는 PC Drive를 설치하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud-SHIELD에는 IRM과 DLP 두 가지 옵션 기능이 있으며, DirectCloud-SHIELD를 계약할 때는 이 중 하나의 옵션 기능을 선택해야 합니다.\
사용자가 DirectCloud 드라이브에서 DirectCloud-SHIELD 기능을 이용하려면, 계약한 옵션 기능에 맞는 애플리케이션을 설치해야 합니다.\
이 매뉴얼 에서는 DirectCloud 지원센터에서 DirectCloud-SHIELD IRM에 대응하는 DirectCloud 드라이브를 다운로드하여 설치하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)은 Windows 대상 64bit 버전만 제공되고 있습니다.\
  Mac용 애플리케이션은 제공되지 않습니다.
* 또한 DirectCloud-SHIELD IRM으로 암호화된 파일은 Windows의 Microsoft Office 애플리케이션에서 직접 열어볼 수 없습니다.\
  아래 방법 중 하나를 사용해 열람해야 합니다.
  * 다음 중 하나를 설치하고, 파일을 더블 클릭하여 열람합니다.\
    DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)\
    DirectCloud-SHIELD IRM PC 전용 애플리케이션
  * DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)를 설치한 뒤, 파일 미리보기 또는 편집을 선택해 열람할 수 있습니다.
* [사용자가 이용할 수 있는 애플리케이션을 제한하는 방법](https://help.directcloud.net/admin_manual/images-and-media/undefined-11)에서 DirectCloud 드라이브가 허용되어 있지 않은 경우, DirectCloud 드라이브에 로그인할 수 없습니다.
* DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)에서는 일반 DirectCloud 드라이브와 동일한 작업을 수행할 수 있습니다.\
  자세한 내용은 [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/directcloud)을 참고해주시기 바랍니다.
*   설치하려는 Windows 버전 DirectCloud 드라이브에 따라 .Net Framework와 Microsoft Edge WebView2 Runtime이 필요할 수 있습니다.\
    추가 설치 필요 여부는 OS에 따라 다릅니다.

    * Windows 10 / 11\
      기본적으로 설치되어 있으므로 추가 설치가 필요하지 않습니다.
    * Windows Server 2019 / 2022\
      .Net Framework는 기본 설치되어 있으나, Microsoft Edge WebView2 Runtime은 설치되어 있지 않습니다.
    * Windows Server 2016\
      .Net Framework와 Microsoft Edge WebView2 Runtime 모두 기본 설치되어 있지 않습니다.

    다만 Microsoft Edge WebView2 Runtime은 Microsoft Office 설치 시 자동으로 설치되므로, 환경에 따라 추가 설치가 필요하지 않을 수도 있습니다.

    추가 설치가 필요한 경우, DirectCloud 드라이브 설치 과정에서 자동으로 설치됩니다.\
    이 때문에 일반적인 설치보다 시간이 더 걸릴 수 있습니다.

    .Net Framework 4.8 및 Microsoft Edge WebView2 Runtime을 추가 설치하려면 인터넷 연결이 가능한 환경이 필요합니다.

### 절차 <a href="#a05" id="a05"></a>

{% hint style="info" %}
**설치 프로그램 다운로드**
{% endhint %}

1. Web 브라우저에서 지원센터를 열고, 아래 주소를 주소창에 입력합니다.\
   [https://directcloud.jp/download](https://directcloud.jp/download)
2. 화면을 아래로 스크롤한 후 DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)의 다운로드 버튼을 클릭합니다.\
   DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)용 설치 프로그램이 다운로드됩니다.

{% hint style="info" %}
**Windows에서 설치 프로그램 실행**
{% endhint %}

1. 다운로드한 설치 프로그램을 더블 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.\
   사용자 계정 컨트롤 화면이 표시된 경우 예를 클릭하면 DirectCloud 드라이브 설정 화면이 표시됩니다.
2. "설치" 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1213).png" alt=""><figcaption></figcaption></figure>

&#x20;      응용 프로그램 설치가 시작됩니다.\
&#x20;      설치가 완료되면 "DirectCloud 드라이브 설정 완료"라는 화면이 표시됩니다.

3. 다시 시작할 시간으로 "지금 재부팅 하겠습니다." 또는 "나중에 재부팅 하겠습니다."을 선택하고 "마침" 버튼을 클릭합니다. '지금 재부팅'을 선택하면 컴퓨터가 즉시 다시 시작됩니다.\
   '나중에 재부팅'을 선택하면 언제든지 컴퓨터를 다시 시작하여 DirectCloud 드라이브(DirectCloud-SHIELD IRM 통합 버전)를 가져올 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1215).png" alt=""><figcaption></figcaption></figure>

4. 다시 시작한 후 바탕 화면에 응용 프로그램 바로 가기가 생성되었는지 확인하십시오.

<figure><img src="../../.gitbook/assets/image (2400).png" alt=""><figcaption></figcaption></figure>
