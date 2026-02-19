---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/cold-storage/auto_move
---

# Cold Storage로 폴더 및 파일이 자동 이동되도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 My Box나 Shared Box 등에서 사용하는 Hot Storage, 장기 보관 시 일부 기능을 제외하여 비용을 낮춘 Warm Storage 외에도 Cold Storage를 제공하고 있습니다.\
Cold Storage는 Warm Storage보다 더 장기 보관에 특화된 Storage입니다. 기능과 데이터 복원과 관련된 일부 제한 사항이 있지만, Warm Storage보다 더 저렴하게 이용할 수 있습니다.\
이 매뉴얼에서는 관리자 페이지에서 Shared Box의 폴더 속성을 표시하여, 파일이 Cold Storage로 자동 이동되도록 설정하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* Warm Storage를 사용할 수 있다 관리자 페이지에 Warm Storage 관리 메뉴가 표시됩니다.
* Cold Storage를 계약한 경우에는 Cold Storage 관리 메뉴가 표시됩니다.
* Warm Storage 또는 Cold Storage 중 하나라도 사용할 수 있는 경우, 폴더 속성에 자동 이동 설정이 표시됩니다.
* Warm Storage와 Cold Storage의 사양에 대해서는, [Warm Storage와 Cold Storage의 차이](https://help.directcloud.net/user_manual/specification/difference_warm_cold)를 참조해 주십시오.
* 자동 이동 대상으로 설정할 수 있는 폴더는 Shared Box의 1단계부터 6단계까지의 폴더에 한정됩니다.
* 상위 폴더에 자동 이동이 설정되어 있는 경우 하위 폴더에 자동 이동 설정이 그대로 상속됩니다. 자동 이동 설정이 상속된 하위 폴더의 폴더 속성에는 자동 이동 변경 버튼이 표시되지 않습니다.
* 하위 폴더에 자동 이동이 설정되어 있는 경우 상위 폴더에서 자동 이동을 사용함으로 설정할 수 없으므로, 상위 폴더의 자동 이동 설정에도 변경 버튼이 표시되지 않습니다.
*   자동 이동은 폴더 단위로 설정합니다.

    예를 들어 아래와 같은 구조의 Shared Box에서 폴더 C에 대해 Cold Storage의 폴더 A로 자동 이동을 설정하면, Cold Storage 폴더 A 안에 폴더 C 이하의 폴더들이 기존 계층 구조를 그대로 유지한 상태로 생성되고, 폴더 C 이하의 파일들이 해당 위치로 이동됩니다.

    <p align="center"><img src="../../.gitbook/assets/image (2265).png" alt=""></p>
* 파일이 Cold Storage로 자동 이동되면, '로그 현황' > '파일의 조작' 메뉴에 '자동 이동' 로그가 기록됩니다.\
  파일이 자동 이동될 때 폴더가 생성된 로그는 기록되지 않습니다.\
  자동 이동 로그를 확인하는 방법에 대해서는, [사용자의 파일 이용 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/log/file_usage_history)을 참조해 주십시오.
* 파일의 자동 이동 대상 위치에 동일한 이름의 폴더가 이미 있는 경우, 해당 폴더로 자동 이동됩니다.
* 자동 이동 대상 위치에 동일한 이름의 파일이 있는 경우, 파일 이름 끝에 숫자가 추가됩니다.
* 자동 이동 대상으로 설정된 Cold Storage 폴더의 이름이나 경로가 변경되면 자동 이동 설정의 이동 위치 정보도 함께 변경됩니다.
* 자동 이동 대상으로 설정된 Cold Storage 폴더가 삭제된 경우, 자동 이동이 실행될 때 자동으로 새 폴더가 생성됩니다.
* 파일이 자동으로 이동되면 다음 정보가 삭제됩니다.
  * 링크 히스토리
  * 파일 잠금
  * 파일 기한
  * 즐겨찾기 정보
  * 전체 검색 데이터
* 다음 정보는 유지됩니다.
  * 태그
  * 버전 이력
  * 코멘트
  * 접근 이력
  * DirectCloud-SHIELD IRM의 기밀 등급 라벨과 irm 확장자
* 마지막 접속 일시가 파일 자동 이동의 기준이 됩니다. 마지막 접속 일시의 다음 날을 기산일로 하며, 기산일을 포함해 이 매뉴얼의 절차에서 설정한 일수가 경과한 뒤 자정 0시부터 순차적으로 파일이 자동 이동됩니다.
* 다음 작업으로 인해 해당 폴더에 저장된 파일에 접근이 발생하면 마지막 접속 일시가 업데이트됩니다.
  * 업로드
  * 덮어쓰기 저장
  * 이름 변경
  * 이동
  * 자동 이동
  * 복사
  * 이전 버전으로 복원
  * 휴지통에서 복원
  * 삭제
  * 자동 삭제(파일 기한)
  * 자동 삭제(My Box)
  * 자동 삭제(폴더 속성)
  * 휴지통
  * 이동 취소
  * 삭제 취소
  * 휴지통 취소
  * 온라인 편집
  * 미리보기
  * DirectCloud 드라이브에서 열기
  * 오프라인 저장
  * 다운로드
  * 첨부 파일 전송
  * 다른 모바일 메일 앱으로 전송
  * 다른 모바일 앱으로 전송
  * 링크 생성\
    \
    이러한 작업에 대한 로그는 로그 > 파일의 조작 메뉴의 액션 항목에서 확인할 수 있습니다.
* 사용자 페이지에서는 파일의 '파일 사용 이력' 화면에서 최종 접근 일시 및 조작 등의 이력을 확인할 수 있습니다.\
  자세한 내용은 [사용자 페이지에서 파일의 사용 이력을 확인하는 방법](https://help.directcloud.net/user_manual/file_management/file_log)을 참조해 주십시오.

### 절차

{% hint style="warning" %}
**자동이동 설정**
{% endhint %}

1. '공유 설정' > 'Shared Box'메뉴를 클릭한 뒤, 자동 이동을 설정하려는 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2276).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 '폴더 옵션' 설정을 표시하고 '자동 이동' 설정을 표시합니다.\
   자동 이동 설정이 없으면 '사용 안함'이 표시됩니다.\
   이미 자동 이동 설정이 되어 있으면 설정 내용이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2267).png" alt=""><figcaption></figcaption></figure>



3. 자동 이동 설정에서 수정 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2268).png" alt=""><figcaption></figcaption></figure>

&#x20;     '자동 이동' 설정이 표시됩니다.



4.  자동 이동의 '사용'에 체크한 뒤, 이동 대상의 “Warm Storage 또는 Cold Storage 폴더를 선택해주세요.”를 클릭합니다.\
    \
    **NOTE**\
    이용 중인 요금제와 옵션 계약 상태에 따라 표시되는 내용이 달라집니다.

    · Warm Storage와 Cold Storage를 모두 사용할 수 있는 경우:\
    &#x20; “Warm Storage 또는 Cold Storage의 폴더를 선택해주세요.”

    · Warm Storage만 사용할 수 있는 경우:\
    &#x20; “Warm Storage의 폴더를 선택해주세요.”

    · Cold Storage만 사용할 수 있는 경우:\
    &#x20; “Cold Storage의 폴더를 선택해주세요.”

<figure><img src="../../.gitbook/assets/image (2277).png" alt=""><figcaption></figcaption></figure>



5. 자동 이동할 파일을 저장할 Cold Storage의 폴더를 선택한 뒤 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2278).png" alt=""><figcaption></figcaption></figure>



6. 파일의 마지막 접속 일시로부터 몇 일이 지난 후 자동 이동할지 드롭다운 목록에서 일수를 선택합니다. 10일부터 2000일까지의 값을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2279).png" alt=""><figcaption></figcaption></figure>



7. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2280).png" alt=""><figcaption></figcaption></figure>

자동 이동 항목에 설정한 내용이 표시됩니다.\
끝에 있는 i 아이콘에 마우스를 올리면, 툴팁으로 이동 대상 폴더를 확인할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2281).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**자동 이동 완료 안내 메일**
{% endhint %}

자동 이동이 설정된 폴더 아래의 파일이 자동으로 이동되면, 이동 원본 폴더에 접근 권한이 있는 모든 사용자에게 “000에서 자동이동이 진행되었습니다.”라는 제목의 이메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (2282).png" alt="" width="499"><figcaption></figcaption></figure>

