---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/custom_settings/custom_domain
---

# 사용자 로그인 페이지의 기본 도메인을 설정하는 방법 (한국미제공)

### 개요 <a href="#a03" id="a03"></a>

기본 도메인을 설정하면 사용자가 가져온 도메인 이름을 사용자 로그인 페이지의 URL에서 사용할 수 있습니다.\
이렇게 하면 사용자가 로그인할 때 회사 ID 입력을 생략할 수 있습니다. 또한 공유 링크 및 게스트 초대 만들기 화면에서 게시된 URL에 자체 도메인을 포함할 수 있습니다.\
이 섹션에서는 사용자 지정 설정 메뉴의 사용자 지정 도메인 설정에서 사용자 로그인 페이지의 기본 도메인을 변경하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 [관리자의 기능 제한](https://boxmanager.directcloud.jp/setting/manager) 으로 "환경 설정"을 선택해야 합니다.
* 계약 플랜이 비즈니스인 경우 유료로 메인 도메인을 이용할 수 있습니다.\
  자세한 내용은 DirectCloud 계약 상황에 따라 아래 문의 양식을 통해 문의하시기 바랍니다.
  * 도입 전 문의\
    [https://directcloud.jp/support/qna\_before](https://directcloud.jp/support/qna_before)
  * 도입 후 문의\
    [https://directcloud.jp/support/qna\_after](https://directcloud.jp/support/qna_after)
* 기본 도메인으로 변경한 후 일반 로그인 URL에 액세스할 수 없도록 차단하는 기능은 없습니다.
* 기본 도메인과 하위 도메인을 모두 설정할 수 없습니다.
* 기본 도메인을 변경하면 공유 링크 및 게스트 초대 URL도 변경됩니다.\
  그러나 기본 도메인을 변경하기 전에 공유 링크에 액세스할 수 있습니다.
* 한 번 설정한 기본 도메인을 변경할 수는 없지만 삭제할 수 있습니다.\
  삭제에 대해서는 [배포 후 문의 양식](https://directcloud.jp/support/qna_after) 에서 문의하시기 바랍니다.

### 절차 <a href="#a05" id="a05"></a>

#### 기본 도메인 설정

1. 환경설정 > 사용자 정의 설정 메뉴를 선택합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMQ8000007JcDf)

2. '사용자 정의 도메인 설정'에서 '기본 도메인 사용'을 선택하고 '로그인 URL'과 '링크 URL'에 검색된 기본 도메인을 입력합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000Puo3)

3. 저장 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000PuoS)

#### 네임서버에 정보 등록하기

로그인 URL, 공유 링크 URL의 값 및 SSL 인증서가 있는 로그인 URL, 공유 링크 URL에 사용되는 레코드 이름 및 값의 발행을 DirectCloud에 요청하고, 발행된 정보를 자신이 관리하는 네임 서버에 등록 합니다.

1. 사용자 지정 도메인 설정의 이름 서버 설정에서 각 레코드의 레코드 이름과 값이 준비 중인지 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000PupQ)

2. [배포 후 문의 양식](https://directcloud.jp/support/qna_after) 에서 이름 서버에 등록할 정보를 게시하도록 DirectCloud에 요청합니다.

72시간 이내에 DirectCloud는 네임서버 구성 정보를 이메일로 전송합니다.

3. 사용자 지정 도메인 설정의 이름 서버 설정에서 각 레코드의 레코드 이름과 값이 표시되는지 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000PuuQ)

4. 72시간 이내에 네임서버에 설정 정보를 등록합니다.

#### DirectCloud에 설정이 반영되는지 확인

DNS 서버에 등록한 후 하루가 경과한 후 다음 화면을 표시하여 설정이 반영되어 있는지 확인합니다.

**사용자 로그인 페이지의 회사 이름**

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000Puuf)

**로그인 URL의 기본 도메인**

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000Puuu)

**사용자 페이지 URL의 기본 도메인**

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000VHmm)

**공유 링크 URL의 기본 도메인**

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000PuvE)

**게스트 초대 URL의 기본 도메인**

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000002fqH\&feoid=00N2w00000JMb2T\&refid=0EMBB000000Puu4)
