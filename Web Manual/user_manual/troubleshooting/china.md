---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/troubleshooting/china
---

# 중국 내에서 DirectCloud에 접근할 수 없는 경우의 해결 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 중국 내에서 DirectCloud에 접근할 수 없는 경우에 대처하는 방법에 대해 설명합니다.

***

### 절차 <a href="#a05" id="a05"></a>

중국 국내에서는 중국 정부의 그레이트 방화벽으로 인해 Amazon Web Services(AWS)에 대한 접근이 제한되어 있습니다.\
일반적인 글로벌 기업의 중국 지사에서는 본사 또는 다른 국가의 사이트와 VPN을 구축하여 이를 회피하고 있습니다.\
VPN 환경이 구축되어 있음에도 불구하고 접근할 수 없는 경우에는 아래의 두 가지 패턴을 고려할 수 있습니다.

{% hint style="warning" %}
**VPN 라우터의 라우팅 설정이 잘못되었습니다.**
{% endhint %}

VPN 라우터의 라우팅 설정에 따라 당사 서버에 연결되지 않을 가능성이 있습니다.\
라우터 설정을 확인해 주시기 바랍니다.



{% hint style="warning" %}
**방화벽에 의해 차단됨**
{% endhint %}

방화벽 설정으로 인해 VPN 경유 데이터 등 특정 패턴이 차단되고 있을 가능성이 있습니다.\
방화벽 설정을 확인해 주시기 바랍니다.
