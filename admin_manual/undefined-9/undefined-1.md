---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-9/undefined-1
---

# 랜섬웨어 방지 기능을 통해 보호하려는 파일의 확장자를 지정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 기본 기능인 랜섬웨어 대책을 사용하시면, 짧은 시간 안에 여러 차례 파일을 변경하는 프로그램을 랜섬웨어로 판단하여 자동으로 차단할 수 있습니다.\
이 매뉴얼에서는, 랜섬웨어로 인한 파일 변경으로부터 보호할 대상을 확장자로 지정하는 방법을 설명합니다.

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

{% hint style="warning" %}
**보호할 파일의 확장자 지정**
{% endhint %}

1. '랜섬웨어 방지' > '설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2157).png" alt=""><figcaption></figcaption></figure>



2. '확장자 정의' 화면에서 보호할 확장자를 텍스트 상자에 입력하고 저장 버튼을 클릭합니다.\
   둘 이상의 확장자를 지정하는 경우 쉼표(,)로 구분하여 입력합니다.

<figure><img src="../../.gitbook/assets/image (2156).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**프로그램이 차단되면**
{% endhint %}

아래 매뉴얼의 절차에 따라 프로그램이 차단되면 "알려지지 않은 프로그램의 파일 변조 시도로 접근을 차단했습니다." 라는 메시지가 표시됩니다. \
또한 프로그램 차단 이력에 로그가 기록됩니다.

* [랜섬웨어 방지 기능을 사용하는 방법](https://help.directcloud.net/admin_manual/undefined-9/undefined)
* [랜섬웨어 방지 기능에서 프로그램이 차단되기까지의 변경 횟수를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-9/undefined-2)
