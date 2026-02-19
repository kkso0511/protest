---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/warm-storage/auto_move_to_warm
---

# 사용자 페이지에서 파일이 Warm Storage로 자동 이동되도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 ‘Warm Storage’를 제공합니다.\
일반적인 Hot Storage에서 링크나 버전 관리 등 일부 기능을 제외한 Warm Storage는 더 저렴한 비용으로 이용할 수 있습니다.\
예를 들어, 자주 사용하지 않는 폴더 계층의 데이터를 모두 Warm Storage로 이동하여 장기 보관하면, Shared Box의 Storage를 효율적으로 활용할 수 있습니다.\
이 매뉴얼에서는 사용자 페이지에서 Shared Box의 폴더 속성을 표시하고, 파일이 Warm Storage로 자동 이동되도록 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 폴더 속성을 설정하는 사용자에게는 <마스터> 접근 권한이 부여되어 있어야 합니다.
* Warm Storage를 이용할 수 있는 경우 사용자 페이지에 ‘Warm Storage’ 메뉴가 표시됩니다.\
  또한, 폴더 속성에 ‘자동 이동’ 설정이 표시됩니다.
* 자동 이동 대상으로 설정할 수 있는 폴더는 1단계부터 6단계까지의 Shared Box 이하에 있는 폴더만 가능합니다.
* 상위 폴더에 자동 이동이 설정되어 있는 경우, 하위 폴더는 해당 설정을 상속받습니다.\
  이렇게 상속된 하위 폴더의 폴더 속성에서는 ‘자동 이동’ 설정에 ‘변경’ 버튼이 표시되지 않습니다.\
  또한, 상위 폴더의 설정에 따라 자동 이동된 하위 폴더의 파일에도 고스트(Ghost)가 표시됩니다.
* 하위 폴더에 자동 이동이 설정되어 있는 경우, 상위 폴더에서는 자동 이동을 ‘사용함’으로 설정할 수 없으므로, 폴더 속성의 ‘자동 이동’ 설정에 ‘설정’ 버튼이 표시되지 않습니다.
* 자동 이동은 폴더 단위로 설정합니다.
* 자동 이동에 관한 로그는 파일의 파일 사용 이력 화면에 다음과 같이 기록됩니다.
  * 파일이 Warm Storage로 자동 이동된 경우: ‘자동 이동’
  * Warm Storage에서 원래 폴더로 파일을 되돌린 경우: ‘이동’
* 파일의 자동 이동 대상 위치에 이미 동일한 이름의 폴더가 있는 경우, 해당 폴더로 파일이 자동 이동됩니다.
* 자동 이동의 이동 원본 폴더 이름이 변경된 경우, 자동 이동이 실행되면 변경된 이름으로 Warm Storage에 새 폴더가 생성되고 파일이 자동 이동됩니다.
* 자동 이동 대상 위치에 동일한 이름의 파일이 있는 경우, 파일 이름 끝에 숫자가 추가됩니다. 이동 원본의 고스트 이름 끝에도 동일하게 숫자가 추가됩니다.
* 자동 이동 대상으로 설정된 Warm Storage의 폴더 이름이나 폴더 경로가 변경된 경우, 자동 이동 설정의 이동 대상 정보도 함께 변경됩니다.
* 자동 이동 대상으로 설정된 Warm Storage 폴더가 삭제된 경우, 자동 이동이 실행될 때 폴더가 자동으로 새로 생성됩니다.
* 파일이 자동 이동되면 다음 정보가 삭제됩니다.
  * 링크 기록
  * 파일 잠금
  * 파일 만료일
* 마지막 접근 날짜가 파일 자동 이동의 기준이 됩니다.\
  마지막 접근 날짜의 다음 날을 기준일로 하여, 그 기준일을 포함해 이 문서의 절차에서 설정한 일수가 경과한 후 자정(0시 0분)부터 순차적으로 파일이 자동 이동됩니다.
*   다음 작업을 통해 대상 폴더에 저장된 파일에 접근이 발생하면, 해당 파일의 마지막 접근 날짜가 갱신됩니다.

    * 업로드
    * 덮어쓰기 저장
    * 이름 변경
    * 이동
    * 자동 이동
    * 복사
    * Cold Storage에서 복원
    * 이전 버전으로 복원
    * 휴지통에서 복원
    * 삭제
    * 자동 삭제(파일 만료일)
    * 자동 삭제(My Box)
    * 자동 삭제(폴더 속성)
    * 휴지통 이동
    * 이동 취소
    * 삭제 취소
    * 휴지통 이동 취소
    * 온라인 편집
    * 미리보기
    * DirectCloud Drive에서 열기
    * 오프라인으로 저장
    * 다운로드
    * 첨부 파일 전송
    * 다른 모바일 메일 앱으로 전송
    * 다른 모바일 앱으로 전송
    * 링크 생성

    이러한 작업의 로그는 파일 사용 이력 화면에서 확인할 수 있습니다.

***

### 절차

{% hint style="warning" %}
**자동 이동 설정**
{% endhint %}

1. 'Shared Box' 메뉴를 클릭하고, 자동 이동을 설정하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 140009.png" alt=""><figcaption></figcaption></figure>



2. 슬라이드 화면의 '폴더 속성' 설정에서 '자동 이동' 설정을 표시합니다.\
   자동 이동이 설정되어 있지 않은 경우 '사용하지 않음'으로 표시됩니다.\
   이미 자동 이동이 설정되어 있는 경우에는 설정 내용이 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 140158.png" alt=""><figcaption></figcaption></figure>



3.  자동 이동 설정의 오른쪽에 표시되는 설정 버튼을 클릭합니다.

    '자동 이동' 설정이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (429).png" alt="" width="563"><figcaption></figcaption></figure>



4. 자동 이동의 '사용함'에 체크하고, '이동할 폴더를 선택하세요.'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (431).png" alt="" width="563"><figcaption></figcaption></figure>



5. 파일의 이동할 폴더를 선택하고 '확인' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (432).png" alt="" width="563"><figcaption></figcaption></figure>



6. 파일의 마지막 접근 일시로부터 며칠이 지난 후 자동으로 이동할지를 드롭다운 목록에서 선택합니다.\
   '10'부터 '2000'까지의 수치를 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (433).png" alt=""><figcaption></figcaption></figure>



7. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (434).png" alt=""><figcaption></figcaption></figure>

'폴더 속성' 설정의 '자동 이동'에 설정한 내용이 표시됩니다.\
끝에 있는 'i' 아이콘에 커서를 올리면, 툴팁에서 이동할 폴더를 확인할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (435).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**자동 이동 완료 이메일 확인**
{% endhint %}

자동 이동이 설정된 폴더 이하의 파일이 자동으로 이동되면, 이동 원본 폴더에 접근 권한이 있는 모든 사용자에게 'ㅇㅇㅇ에서 자동 이동이 진행 되었습니다.'라는 제목의 메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (436).png" alt="" width="375"><figcaption></figcaption></figure>
