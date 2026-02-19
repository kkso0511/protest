---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/storage/check_file_in_trash
---

# 사용자의 My Box 및 휴지통에 저장된 파일을 확인 하는 방법(한국미제공) (감사옵션)

### 개요 <a href="#a03" id="a03"></a>

이 섹션에서는 DirectCloud 감사를 사용하는 경우 관리 페이지에서 아래에 저장된 파일을 미리 보는 방법에 대해 설명합니다.

* 사용자의 내 상자 및 휴지통
* 게스트 및 Connect User 휴지통

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 [관리자의 기능 제한](https://boxmanager.directcloud.jp/setting/manager) 으로 "저장소"를 선택해야 합니다.
* 계약 계획이 엔터프라이즈인 경우 DirectCloud의 무료 옵션인 DirectCloud 감사를 사용할 수 있습니다.
* DirectCloud 감사를 한 번 활성화하면 비활성화된 상태로 되돌릴 수 없습니다.
* DirectCloud 감사를 사용하면 삭제된 사용자의 ID를 다시 활성화할 수 없습니다. 또한 삭제된 사용자 ID로 사용자를 다시 추가할 수 없습니다.
* 게스트 및 Connect User의 내 상자에 저장된 파일을 미리 볼 수 없습니다.
* 다음 화면에서는 폴더와 파일을 삭제할 수 없습니다. 사용자 페이지에서 삭제해야 합니다.
  * "저장소" > "사용자 할당량"메뉴의 "내 상자 사용"
  * "저장소"> "게스트 휴지통"메뉴
  * 스토리지 > Connect User 휴지통 메뉴
* 파일을 미리 보면 로그 > 감사 활동 로그에 감사 담당자의 작업 내역이 기록됩니다.\
  자세한 내용은 [감사 활동 로그를 확인하는 방법을](https://help.directcloud.jp/s/article/operation-of-administrator-function11208) 참조하십시오.
* 이 문서의 단계에서 파일을 미리 보는 사용자는 [사용자에게 감사 담당자 권한을 부여하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11202) 의 절차에 따라 감사 담당자로 설정되어 있어야 합니다.
* 감사 담당자로 설정된 사용자에게는 [사용자에게 일반 관리자 권한을 추가하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11119) 의 단계에서 일반 관리자 권한이 부여되어야 합니다.
* 감사 담당자는 관리자의 모든 기능을 이용할 수 있습니다. [일반 관리자가 사용할 수 있는 메뉴를 제한하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11122) 에 따라 감사 담당자의 관리 페이지에 표시되는 메뉴를 제한할 수 없습니다.
* 내보낼 CSV 파일의 문자 코드는 환경 설정 > 고급 설정 메뉴의 내보내기 시 문자 코드 설정에서 설정됩니다.\
  자세한 내용은 [내보낼 파일의 문자 코드를 설정하는 방법](https://help.directcloud.jp/s/article/operation-of-administrator-function11267) 을 참조하십시오.

### 절차 <a href="#a05" id="a05"></a>

#### 사용자의 내 상자 및 휴지통에 있는 파일 미리보기

1. 스토리지 > 사용자 할당량 메뉴를 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMQ8000005huIc)

2. 파일을 미리 보려는 사용자의 사용량 열에 표시되는 파일 목록 버튼을 클릭합니다.\
   사용자가 많으면 '검색' 또는 '정렬'을 사용하여 원하는 사용자를 표시하는 것이 좋습니다.

![002\_tr\_45%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a92j)

"내 상자 사용"이 표시됩니다.

![002\_tr\_45%.png](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9JZ)

| 품목       | 설명                                                                                                                                 |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| 파일/폴더 이름 | <p>폴더 또는 파일의 이름이 표시됩니다.<br>이름의 오름차순/내림차순으로 정렬할 수 있습니다.</p>                                                                         |
| 일시       | <p>폴더의 경우 업로드 또는 생성된 날짜와 시간이 표시됩니다.<br>파일의 경우 업로드된 날짜와 시간이 표시됩니다.<br>날짜와 시간의 오름차순/내림차순으로 정렬할 수 있습니다.</p>                           |
| 사이즈      | <p>파일의 크기가 표시됩니다.<br>폴더의 경우 크기는 비어 있습니다.</p>                                                                                       |
| 브라우징 기록  | <p>파일을 본 횟수가 표시됩니다.<br>폴더의 경우는 공란이 됩니다.<br>클릭하면 브라우징 기록 화면에서 파일을 본 사용자를 볼 수 있습니다.</p>                                              |
| 링크 내역    | <p>폴더나 파일 링크가 생성된 횟수가 표시됩니다.<br>첫 번째 계층의 폴더는 링크가 생성되지 않기 때문에 "0"으로 표시됩니다.<br>클릭하면 링크 내역 화면에서 링크를 만든 사용자, 링크 URL 등을 확인할 수 있습니다.</p> |

3. '내 상자 사용'에서 사용자의 내 상자에 있는 폴더를 선택하고 미리 보려는 파일을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9Jt)

파일 미리보기 화면이 표시됩니다.\
왼쪽 하단의 다운로드 버튼을 클릭하면 파일을 다운로드할 수 있습니다.\
파일 미리보기 화면을 닫으려면 오른쪽 상단의 ✕ 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a8mI)

4. 휴지통 파일을 미리 보려면 '내 상자 사용'에서 '○○(사용자 이름) 휴지통'을 클릭한 다음 파일을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9GD)

파일 미리보기 화면이 표시됩니다.\
왼쪽 하단의 다운로드 버튼을 클릭하면 파일을 다운로드할 수 있습니다.\
파일 미리보기 화면을 닫으려면 오른쪽 상단의 ✕ 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a8s2)

#### 게스트 또는 Connect User 휴지통에 있는 파일 미리보기

이 문서에서는 게스트 또는 Connect User 휴지통에 있는 파일을 미리 보는 절차에 대해 설명합니다.\
아래에서는 "게스트 휴지통" 화면을 사용하여 설명합니다. "Connect User 휴지통"에서도 유사한 절차를 사용하여 파일을 미리 볼 수 있습니다.

**게스트/Connect User 휴지통 보기**

1. 다음 방법 중 하나로 게스트 또는 Connect User 휴지통을 표시합니다.

❶  게스트 휴지통을 보려면 저장 > 게스트 휴지통 메뉴를 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMQ8000005hwXJ)

❷  Connect User 휴지통을 보려면 스토리지 > Connect User 휴지통 메뉴를 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMQ8000005htmM)

**게스트/Connect User 휴지통 파일 미리보기**

1. 게스트 휴지통 또는 연결 사용자 휴지통에서 미리 보려는 파일을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9KX)

파일 미리보기 화면이 표시됩니다.\
왼쪽 하단의 다운로드 버튼을 클릭하면 파일을 다운로드할 수 있습니다.\
파일 미리보기 화면을 닫으려면 오른쪽 상단의 ✕ 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9Kh)

**게스트/Connect User의 휴지통 폴더와 파일을 좁히고 표시**

'게스트 휴지통' 또는 '연결 사용자 휴지통'을 사용하면 휴지통 폴더와 파일을 기간, 사용자, 파일 이름 및 수로 필터링하여 볼 수 있습니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9Km)

| No. | 설명                                                                                                                                                                           |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ❶   | '게스트 휴지통' 또는 '연결 사용자 휴지통' 폴더 및 파일을 표시하는 기간을 최근 7일, 최근 15일, 최근 1개월, 최근 3개월 중에서 선택합니다.                                                                                         |
| ❷   | <p>계약 시작부터 현재까지 '게스트 휴지통' 또는 '연결 사용자 휴지통'으로 이동한 폴더 및 파일을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.<br>그러나 2024년 1월에 시작한 신규 요금 플랜에서 표준 플랜과 고급 플랜을 계약한 경우에는 이 설정이 표시되지 않습니다.</p> |
| ❸   | 게스트 휴지통 또는 연결 사용자 휴지통 폴더 및 파일을 필터링하려면 사용자 이름, 사용자 ID 및 파일 이름을 입력합니다.                                                                                                         |
| ❹   | "게스트 휴지통" 또는 "연결 사용자 휴지통" 폴더 및 파일을 표시할 수를 "10", "25", "50", "100" 중에서 선택합니다.                                                                                                 |

**게스트/Connect User 휴지통 폴더 및 파일 정보를 CSV 파일로 내보내기**

1. 게스트 휴지통 또는 연결 사용자 휴지통에서 CSV 내보내기 버튼을 클릭합니다.\
   필요한 경우 휴지통 폴더/파일 정보를 좁히고 내보내는 것이 좋습니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9Kw)

CSV 파일이 다운로드됩니다.

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001iIL\&feoid=00N2w00000JMb2T\&refid=0EMBB000000a9Kx)
