---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-15/undefined
---

# 사용자 페이지에 로그인할 수 없는 경우 해결 방법

### 개요 <a href="#a03" id="a03"></a>

사용자 페이지에 로그인할 수 없는 경우에는 발생 상황을 확인한 후, 가장 적절한 대처 방법을 시도해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**모든 애플리케이션**
{% endhint %}

DirectCloud는 AWS(Amazon Web Services)의 ELB(Elastic Load Balancing)를 사용하여 부하 분산을 수행하고 있으므로, 접속 대상 IP 주소는 사전 예고 없이 비정기적으로 변경됩니다.\
따라서 IP 주소가 아닌 도메인 기준으로 접근 제어를 설정해야 합니다.\
접속하는 네트워크의 방화벽 또는 프록시 서버에서 아래의 포트 번호 및 도메인으로의 통신을 허용하도록 설정해 주시기 바랍니다.

**\[포트 번호]**

포트 번호: 443\
프로토콜: HTTPS



**\[도메인]**

사양 또는 네트워크 구성 변경으로 인해 새로운 도메인이 추가되거나 기존 도메인이 변경될 수 있습니다.\
이 경우, 추가되거나 변경된 도메인으로의 통신을 허용하도록 설정해야 합니다.\
통신 허용이 필요한 도메인에 대해서는 [DirectCloud 공통 사양](https://help.directcloud.net/user_manual/undefined-14/directcloud)의 포트 번호 및 도메인 액세스 제어 정보를 참고해 주시기 바랍니다.



**\[IP 주소로 제어해야 하는 경우]**

시스템이 포트 번호나 도메인 제어를 지원하지 않는 등 IP 주소로 제어해야 하는 경우 Amazon Web Services 지원 페이지에 게시된 IP 주소 범위에서 DirectCloud에서 사용 할 IP 주소를 모두 허용해야 합니다.

* Amazon Web Services의 IP 주소 범위\
  https://docs.aws.amazon.com/ko\_kr/general/latest/gr/aws-ip-ranges.html#subscribe-notifications
* 게시된 JSON 파일 다운로드 링크\
  https://ip-ranges.amazonaws.com/ip-ranges.json

게시된 JSON 파일을 참조하고 DirectCloud가 사용하는 다음 IP 주소 범위와 통신할 수 있도록 방화벽, 프록시 서버 등을 구성합니다.

* "region": "ap-northeast-1"
* "service": "AMAZON"
* "network\_border\_group": "ap-northeast-1"

또한 AWS가 게시하는 IP 주소의 범위는 예고 없이 부정기적으로 변경될 수 있습니다.\
이 IP 주소 범위가 변경되면 위의 JSON 파일을 다시 가져와 대상 IP 주소 범위를 기반으로 방화벽 및 프록시 서버 설정을 업데이트해야 합니다.



{% hint style="warning" %}
**Web 브라우저**
{% endhint %}

Web 브라우저에서 사용자 페이지에 접속이 되지 않는 경우 브라우저의 쿠키와캐시 삭제를 시도하여 해결 할 수도 있습니다.

1. 사용중인 인터넷 브라우저를 실행한 상태에서 키보드의 ctrl + Shift + Del 키를 동시에 누릅니다.
2. 나타나는 데이터 삭제 창에서 기간 혹은 시간을 모든기간 혹은 전체 로 선택을 합니다.
3. 아래 삭제 할 항목에서 쿠키와 캐시를 선택하고 전체삭제를 실행합니다.



{% hint style="warning" %}
**DirectCloud 드라이브(Windows, Mac)**
{% endhint %}

DirectCloud 드라이브에 로그인하면 '서버에 연결 중'이 표시될 수 있습니다.\
이 경우 다음 단계를 시도해 보십시오.

1. DirectCloud 드라이브를 제거하고 다시 설치
2. 운영 체제를 최신 패치가 적용된 상태로 업데이트
