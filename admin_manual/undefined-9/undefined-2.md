---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-9/undefined-2
---

# 랜섬웨어 방지 기능에서 프로그램이 차단되기까지의 변경 횟수를 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 기본 기능인 랜섬웨어 대책을 사용하시면, 짧은 시간 안에 여러 차례 파일을 변경한 프로그램을 랜섬웨어로 판단하여 자동으로 차단할 수 있습니다.\
이 매뉴얼에서는 프로그램을 차단하는 조건을, 파일에 접근하여 변조 하려는 횟수로 지정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 랜섬웨어 방지 기능은 모든 요금제에서 추가 비용 없이 이용할 수 있습니다.
* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '랜섬웨어 방지' 항목에 접근 가능합니다.
* 랜섬웨어 방지 기능으로 차단되는 대상은 DirectCloud 드라이브에 저장된 파일을 변경한 프로그램만 해당됩니다. 파일을 열기만 한 경우에는 변경으로 판단되지 않습니다.
* 프로그램이 첫 번째 파일을 연 시점부터 10초 이내에 프로그램 차단 정책 설정에서 지정한 수 이상의 파일을 변경한 경우, 해당 프로그램은 차단됩니다.
* 한 번 프로그램이 차단 프로그램으로 등록되면, 동일한 프로그램이 파일을 열기만 해도 변경으로 판단됩니다.
* 디지털 서명이 포함된 프로그램은 이 기능으로 차단할 수 없습니다.
* macOS용 DirectCloud 드라이브에서는 랜섬웨어 방지 기능을 이용할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="info" %}
**프로그램의 차단 규칙 횟수 지정**
{% endhint %}

1. '랜섬웨어 방지' > '설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2159).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 프로그램 차단 규칙 에서 파일 수를 4에서 20 사이의 숫자를 설정한 다음 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2158).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**프로그램이 차단되면**
{% endhint %}

아래 매뉴얼의 절차에 따라 프로그램이 차단되면 "알려지지 않은 프로그램의 파일 변조 시도로 접근을 차단했습니다." 라는 메시지가 표시됩니다. \
또한 프로그램 차단 이력에 로그가 기록됩니다.

* [랜섬웨어 방지 기능을 사용하는 방법](https://help.directcloud.net/admin_manual/undefined-9/undefined)
* [랜섬웨어 방지 기능에서 프로그램이 차단되기까지의 변경 횟수를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-9/undefined-2)
