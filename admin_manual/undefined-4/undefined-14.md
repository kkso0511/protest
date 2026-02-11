---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-4/undefined-14
---

# 폴더의 권한 정보를 대량으로 내보내는 방법 (한국미제공)

### 개요 <a href="#a03" id="a03"></a>

이 섹션에서는 환경 설정 > Connect 관리 메뉴의 액세스 권한 일괄 처리 설정에서 공유 폴더 및 Connect 폴더의 액세스 권한 정보 목록을 CSV 파일로 일괄 내보내는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 기사에서는 환경 설정 메뉴의 공유 및 연결 관리 메뉴를 설정하는 방법에 대해 설명합니다. 수 있습니다.
* 관리자 권한이 부여된 사용자는 [관리자의 기능 제한](https://boxmanager.directcloud.jp/setting/manager) 으로 "환경 설정"을 선택해야 합니다.
* 사용자 액세스 권한 설정 및 게스트 액세스 권한 설정 화면에서 사용자 그룹 게스트 액세스 권한을 삭제 한 후 액세스 권한을 내보낼 때 액세스 권한을 삭제 한 사용자의 권한 열에 "noAccess"가 표시됩니다.
* '사용자 액세스 권한 설정' 화면에서 '상위 계층의 액세스 권한을 상속하지 않음'을 선택하면 액세스 권한을 내보낼 때 대상 폴더의 '상위 계층의 권한 상속하지 않음'으로 'Y'가 들어가서, 「권한」열은 공란이 됩니다.
* 대상 사용자가 "지정한 사용자"로 설정된 폴더에 대한 액세스 권한 정보만 내보내집니다.
* CSV 파일로 내보낼 수 있는 액세스 권한 정보의 행 수에 대한 제한은 모든 계획에서 일률적으로 1,000,000행입니다.
* 여러 내보내기를 요청할 수 있지만 연속 처리 시간이 3시간을 초과하면 오류가 발생합니다.
* 계약 플랜이 비즈니스 이상이고 DirectCloud의 무료 옵션인 "DirectCloud 전자장부 보존법 대응"을 이용할 수 있는 경우 관리 페이지의 "환경 설정" > "문서 관리" 메뉴에서 액세스 권한 정보를 일괄적으로 내보내는 것 수 있습니다.
* 문서 관리 메뉴의 폴더에서는 게스트를 초대할 수 없습니다.\
  따라서 문서 관리 메뉴의 액세스 권한 일괄 처리에서 내보낸 CSV 파일에는 게스트 ID가 포함되지 않습니다.
* 계약 플랜이 엔터프라이즈이고 DirectCloud의 무료 옵션인 DirectCloud-CONNECT를 사용할 수 있는 경우 관리 페이지의 환경설정 > Connect 관리 메뉴에서 액세스 권한 정보를 일괄적으로 내보낼 수 있습니다.
* Connect 폴더의 액세스 권한 정보를 내보낼 때 CSV 파일의 헤더에 "Connect User"가 표시되지 않습니다.
* 계약 플랜이 비즈니스 이상이고 DirectCloud 유료 옵션인 DirectCloud-SHIELD DLP를 계약하는 경우 관리 페이지의 환경 설정 > DLP 관리 메뉴에서 액세스 권한 정보를 일괄 내보내는 것 수 있습니다.
* 계약 계획이 비즈니스 이상이고 DirectCloud의 유료 옵션인 "웜 스토리지"를 계약하는 경우 관리 페이지의 "환경 설정" > "웜 스토리지 관리" 메뉴에서 액세스 권한 정보를 일괄적으로 내보낼 수 있습니다. 수 있습니다.
* 내보낼 CSV 파일의 문자 코드는 환경 설정 > 고급 설정 메뉴의 CSV 내보내기 시 문자 코드 설정에서 설정됩니다.\
  자세한 내용은 [내보낼 CSV 파일의 문자 코드를 설정하는 방법을](https://help.directcloud.jp/s/article/operation-of-administrator-function11267) 참조하십시오.

### 절차 <a href="#a05" id="a05"></a>

#### 공유 폴더의 액세스 권한 정보를 일괄 출력

**액세스 권한 정보 내보내기 요청**

1. 환경설정 > 공유 메뉴를 선택하고 액세스 권한 일괄 처리 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004awRO)

2. CSV 내보내기 설정을 표시하고 CSV 내보내기 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004ayWQ)

3. CSV 요청 확인 화면에서 출력 행 수와 문자 코드를 확인한 다음 요청 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004azyl)

CSV 내보내기 처리가 완료되면 요청한 계약 담당 관리자 또는 일반 관리자의 이메일 주소로 알림 이메일을 받게 됩니다.

**알림 이메일 링크에서 CSV 파일 다운로드**

1. 알림 이메일을 표시하고 '다운로드 URL'을 클릭합니다.\
   또는 관리 페이지에 로그인한 후 다음 URL을 주소 표시줄에 붙여넣어 직접 액세스할 수 있습니다.\
   [https://boxmanager.directcloud.jp/csv/list](https://boxmanager.directcloud.jp/csv/list)

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004azFa)

CSV 파일 다운로드 페이지가 표시됩니다.

2. CSV 내보내기 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004azDz)

CSV 파일이 다운로드됩니다.

3. CSV 파일을 보고 액세스 권한 정보를 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004avgc)

#### Connect 폴더의 액세스 권한 정보를 일괄 출력

**액세스 권한 정보 내보내기 요청**

1. 환경설정 > Connect 관리 메뉴를 선택하고 액세스 권한 일괄 처리 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004asE6)

2. CSV 내보내기 설정을 표시하고 CSV 내보내기 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004axTv)

3. CSV 요청 확인 화면에서 출력 행 수와 문자 코드를 확인한 다음 요청 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004b1pG)

CSV 내보내기 처리가 완료되면 요청한 계약 담당 관리자 또는 일반 관리자의 이메일 주소로 알림 이메일을 받게 됩니다.

**알림 이메일 링크에서 CSV 파일 다운로드**

1. 알림 이메일을 표시하고 '다운로드 URL'을 클릭합니다.\
   또는 관리 페이지에 로그인한 후 다음 URL을 주소 표시줄에 붙여넣어 직접 액세스할 수 있습니다.\
   [https://boxmanager.directcloud.jp/csv/list](https://boxmanager.directcloud.jp/csv/list)

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004b2Oj)

CSV 파일 다운로드 페이지가 표시됩니다.

2. CSV 내보내기 버튼을 클릭합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004avaA)

CSV 파일이 다운로드됩니다.

3. CSV 파일을 보고 액세스 권한 정보를 확인합니다.

![이미지](https://help.directcloud.jp/servlet/rtaImage?eid=ka0Q80000001H6r\&feoid=00N2w00000JMb2T\&refid=0EMQ8000004b2Rx)
