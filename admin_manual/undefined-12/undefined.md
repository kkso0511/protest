---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-12/undefined
---

# 장애가 발생한 경우의 대응에 대해 (한국에 맞게 내용 업데이트 필요)

### 개요 <a href="#a03" id="a03"></a>

이 섹션에서는 DirectCloud 서비스에 장애로 인한 문제가 발생한 경우 어떤 흐름으로 대응하는지 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 다음과 같은 경우에는 SLA(Service Level Agreement)에 따른 감액의 대상이 되지 않습니다.
  * DirectCloud에 연결하기 위한 회선에 장애가 발생한 경우
  * 직접 클라우드의 관리되지 않는 장비로 인해 장애가 발생한 경우
  * 다음 업데이트 및 유지 보수로 DirectCloud가 유지 보수 작업을 수행하는 경우\
    주요업데이트, 간단한 업데이트, 임시 업데이트, 정기 유지보수, 임시 유지보수
  * 천재 재해, 역병의 만연, 악의의 제삼자에 의한 방해 행위에 의해, 장해가 발생했을 경우
  * 이용약관이 정하는 의무에 위배하는 행위로 인해 장애가 발생한 경우

### 설명 <a href="#a05" id="a05"></a>

#### 애플리케이션에 결함이 발생한 경우

* 관리 페이지\
  [https://boxmanager.directcloud.jp/#/list](https://boxmanager.directcloud.jp/#/list)
* 사용자 페이지\
  [https://web.directcloud.jp/notice](https://web.directcloud.jp/notice)
* 지원 페이지\
  [https://directcloud.jp/support/maintenance](https://directcloud.jp/support/maintenance)

그 후, 원인이 특정되는 대로, 「임시 메인터넌스의 알림」이라고 하는 타이틀로, 메인터넌스의 실시 일시와 메인터넌스 내용을 고지합니다.\
응용 프로그램으로 인한 오류가 발생하면 서비스를 중지하지 않고 유지 관리 작업을 수행합니다.

#### 서버에 결함이 발생한 경우

관리 페이지, 사용자 페이지의 "장애 및 유지 보수 정보"및 지원 페이지의 "유지 관리 정보"에 결함을 알립니다.

* 관리 페이지\
  [https://boxmanager.directcloud.jp/#/list](https://boxmanager.directcloud.jp/#/list)
* 사용자 페이지\
  [https://web.directcloud.jp/notice](https://web.directcloud.jp/notice)
* 지원 페이지\
  [https://directcloud.jp/support/maintenance](https://directcloud.jp/support/maintenance)

그 후, 원인 및 대처 방법이 확정되는 대로, 「임시 메인터넌스의 알림」이라고 하는 타이틀로, 메인터넌스의 실시 일시와 메인터넌스 내용을 고지합니다.\
서버로 인한 오류가 발생하면 서비스를 중지하고 유지 관리 작업을 수행합니다.\
월간 서버 가동률이 99.95 미만이 되었을 경우, 다이렉트 클라우드에서는 품질 보증 제도(SLA)에 근거해 이용 요금의 감액 대응을 실시하고 있습니다만, 이하의 업데이트 및 메인터넌스에 따른 서비스 정지는 카운트되지 않습니다.

* 주요 업데이트
* 사소한 업데이트
* 임시 업데이트
* 정기 유지 보수
* 임시 유지 보수

도쿄 리전 내의 데이터 센터 1 거점의 파괴 등에 의해 데이터가 소실된 경우, 다른 거점으로부터 WAN 경유로 복원을 실시합니다.\
목표 복구 시간(RTO: Recovery Time Objective)과 목표 복구 지점(RPO: Recovery Point Objective)은 모두 24시간 이내입니다.\
DR(Disaster Recovery) 사이트에서 복원할 수 없습니다.\
\
SLA와 관련된 감액 신청은 시스템이 복구된 날부터 다음 달 20일까지 절차를 거쳐야 합니다.\
자세한 내용은 다음 페이지를 참조하십시오.\
[https://directcloud.jp/sla](https://directcloud.jp/sla)
