---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/account_settings/d_log
---

# DirectCloud 드라이브의 로그를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud 드라이브에서 문제가 발생했을 때, 로그 파일을 첨부하여 문의하시면 문제가 해결될 수 있습니다. 일반 로그로는 해결이 어려운 경우, 디버그 모드에서 DirectCloud 드라이브를 실행하면 보다 상세한 정보를 로그 파일에 출력할 수 있습니다.\
이 매뉴얼에서는 DirectCloud 드라이브의 로그 폴더를 표시하는 방법과 디버그 모드에서 DirectCloud 드라이브를 실행하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

*   디버그 모드 실행을 통한 로그 수집은 다음 애플리케이션에서 이용할 수 있습니다.

    <table><thead><tr><th width="163">OS</th><th width="167.20001220703125">애플리케이션 유형</th><th>프로그램</th></tr></thead><tbody><tr><td>윈도우</td><td>일반 버전</td><td><ul><li>DirectCloud 드라이브</li></ul></td></tr><tr><td></td><td>통합 버전</td><td><ul><li>DirectCloud-SHIELD IRM 통합 버전</li><li>DirectCloud-SHIELD DLP 통합 버전</li></ul></td></tr><tr><td>macOS</td><td>일반 버전</td><td><ul><li>DirectCloud 드라이브</li></ul></td></tr></tbody></table>
* 이 매뉴얼에서는 Windows용 DirectCloud 드라이브를 예로 들어 설명하고 있습니다.
* macOS용 DirectCloud 드라이브의 로그 저장 폴더에 대해서는 자주 묻는 질문의 “각 애플리케이션의 로그 저장 위치를 알려주세요.” 항목을 참고하시기 바랍니다.
* 디버그 모드에서 DirectCloud 드라이브를 실행 중 로그아웃하면 디버그 모드는 종료됩니다.
* 또한 디버그 모드에서 DirectCloud 드라이브를 실행하면 성능이 저하될 수 있습니다. 문제가 재현되어 디버그 로그를 수집한 후에는 즉시 디버그 모드를 종료하실 것을 권장드립니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**DirectCloud 드라이브의 로그 폴더 보기**
{% endhint %}

이 매뉴얼에서는 DirectCloud 드라이브에 로그인한 상태에서 로그 폴더를 표시하는 방법을 설명합니다.

1. DirectCloud 드라이브에 로그인합니다.



2. 설정 화면 오른쪽 상단에 있는 '⁝' 버튼을 클릭한 뒤, 표시된 상세 설정 메뉴에서 '로그 폴더 열기'를 선택합니다.

<figure><img src="../../.gitbook/assets/image (801).png" alt=""><figcaption></figcaption></figure>

Windows 탐색기에서 Windows에 로그인한 사용자의 폴더 아래에 있는 DirectCloud 드라이브의 로그 폴더가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (803).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브를 디버그 모드로 실행**
{% endhint %}

DirectCloud 드라이브에 로그인한 상태에서 DirectCloud 드라이브를 디버그 모드로 실행합니다.

1. 설정 화면의 오른쪽 상단에 있는 '⁝' 버튼을 클릭하고 표시된 고급 설정 메뉴에서 '디버그 모드로 실행'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (804).png" alt=""><figcaption></figcaption></figure>



2. 디버그 모드에서 실행하기 위한 확인 대화 상자가 표시됩니다.\
   '예' 버튼을 클릭합니다.\
   DirectCloud 드라이브가 재시작되어 디버그 모드로 실행됩니다.\
   로그인 화면의 ‘로그인 상태 유지’에 체크되어 있는 경우에는 DirectCloud 드라이브에 자동으로 로그인됩니다. 로그인 화면이 표시된 경우에는 DirectCloud 드라이브에 로그인해 주십시오.

<figure><img src="../../.gitbook/assets/image (805).png" alt=""><figcaption></figcaption></figure>



3. 설정 화면을 열고, 조작 버튼 아래에 ‘디버그 모드 실행 중’이라는 문구가 표시되어 있는지 확인합니다.\
   DirectCloud 드라이브가 디버그 모드로 실행되는 동안에는 확장자가 ‘debug’인 파일에 상세한 로그가 기록됩니다.

<figure><img src="../../.gitbook/assets/image (807).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브의 디버그 모드 종료**
{% endhint %}

DirectCloud 드라이브의 디버그 모드를 종료합니다.

1. 조작 버튼 아래에 표시된 "디버그모드 실행중"을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (808).png" alt=""><figcaption></figcaption></figure>



2. 디버그 모드를 종료하는 확인 대화 상자가 표시됩니다.\
   '예' 버튼을 클릭합니다.\
   DirectCloud 드라이브가 재시작되면서 디버그 모드가 종료됩니다.\
   로그인 화면의 ‘로그인 상태 유지’에 체크되어 있는 경우에는 DirectCloud 드라이브에 자동으로 로그인됩니다. 로그인 화면이 표시된 경우에는 DirectCloud 드라이브에 로그인해 주십시오.

<figure><img src="../../.gitbook/assets/image (809).png" alt=""><figcaption></figcaption></figure>

