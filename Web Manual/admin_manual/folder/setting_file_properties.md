---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/folder/setting_file_properties
---

# 파일에 부여할 문서 속성의 항목을 설정하는 방법 (한국미제공)

### 개요 <a href="#a03" id="a03"></a>

DirectCloud는 전자장부 보존법(전장법)의 개정으로 2024년 1월 이후에 의무화되는 전자거래 데이터의 전자보존에 대응하고 있습니다.\
DirectCloud 전자장부 보존법 대응을 이용함으로써 사용자는 문서 관리 메뉴에서 전자장부 보존법에 의해 정해진 요건에 따라 국세관계 서류를 파일로 관리할 수 있습니다.\
이 절에서는 관리 페이지의 문서 관리 메뉴에서 파일에 부여할 문서 속성의 항목을 설정하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 [관리자의 기능 제한](https://boxmanager.directcloud.jp/setting/manager) 으로 "환경 설정"을 선택해야 합니다.
* 비즈니스 플랜, 프리미엄 플랜 또는 엔터프라이즈 플랜 중 하나를 계약하는 경우 DirectCloud 전자장부 보존법을 무료로 사용할 수 있습니다.
* DirectCloud 전자장부 보존법 대응에 대한 자세한 내용은 DirectCloud 배포 상황에 따라 아래 문의 양식을 통해 문의하시기 바랍니다.\
  배포 전 문의:\
  [https://directcloud.jp/support/qna\_before](https://directcloud.jp/support/qna_before)\
  도입 후 문의:\
  [https://directcloud.jp/support/qna\_after](https://directcloud.jp/support/qna_after)
* 문서 속성 설정에서 항목을 "필수 필수"로 설정하려면 사용을 선택해야 합니다.
* 개정 전자장부 보존법에서는, 「거래 연월일」 「거래처」 「거래 금액」으로 서류를 검색할 수 있는 상태가 되어 있을 필요가 있기 때문에, 문서 속성의 항목 설정으로 이러한 체크를 제외할 수 없습니다 .
* 전자장부 보존법에 대응하려면 국세관계 서류의 보존 요건에 따라 DirectCloud 전자장부 보존법 대응 기능을 운용해야 합니다.\
  전자장부 보존법에 대응한 운용 방법에 대해서는, 이하의 문서를 참조해 주세요.
  * [전자장부 보존법 대응 DirectCloud 운용 매뉴얼(스캐너 보존)](https://link.directcloud.jp/9MOulJb6oY)
  * [전자장부 보존법 대응 DirectCloud 운용 매뉴얼(전자 거래)](https://link.directcloud.jp/dKKIVh5ybW)

### 절차 <a href="#a05" id="a05"></a>

#### 문서 속성의 항목 설정

1. 공유 > 문서 관리 메뉴를 클릭합니다.

![영상](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000107d\&feoid=00N2w00000JMb2T\&refid=0EMBB000000ndlj)

2. 화면을 아래로 스크롤하고 문서 속성 설정에서 문서 관리 폴더의 파일에 추가할 문서 속성 항목을 설정합니다.

![영상](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000107d\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001QqLl)

| 프로젝트  | 설명                                                                                                                                                                                                    |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 속성 이름 | <p>파일에 설정할 수 있는 문서 속성의 이름이 표시됩니다.</p><ul><li>문서 유형</li><li>거래 연월일</li><li>비즈니스 파트너</li><li>거래 금액</li><li>사업자등록번호</li><li>메모</li></ul>                                                                 |
| 사용    | 문서 관리 폴더의 파일에 설정하려는 문서 속성의 항목을 체크합니다.                                                                                                                                                                 |
| 입력 필수 | 문서 속성을 입력해야 하는 경우 선택합니다.                                                                                                                                                                              |
| 작동하다  | <p>"문서 유형"의 "작업"에 표시된 버튼을 클릭하여 파일에 등록할 수 있도록 하는 문서 유형을 선택합니다.<br>선택할 수 있는 문서 종류는 다음과 같습니다.</p><ul><li>계약서</li><li>납품서</li><li>송장</li><li>영수증</li><li>견적서</li><li>주문서</li><li>주문서</li><li>송장</li></ul> |

3. 저장 버튼을 클릭합니다.

![영상](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000107d\&feoid=00N2w00000JMb2T\&refid=0EMQ8000001QqOz)

#### 사용자 페이지에서 문서 속성 표시 예

관리자가 설정한 문서 속성 항목은 파일 미리보기를 볼 때 오른쪽의 "문서 속성"에 표시됩니다.

![영상](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000107d\&feoid=00N2w00000JMb2T\&refid=0EMBB000000ndoN)

문서 속성 정보가 등록되지 않은 경우에는 "문서 속성이 등록되지 않았습니다."가 표시됩니다. 등록 버튼을 클릭하면 문서 속성 정보를 설정할 수 있습니다.

![영상](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q8000000107d\&feoid=00N2w00000JMb2T\&refid=0EMBB000000ndoS)
