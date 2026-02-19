---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/warm-storage/auto_move
---

# Warm Storage로 폴더 및 파일이 자동 이동되도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 ‘Warm Storage’를 제공합니다.\
일반적인 Hot Storage에서 링크나 버전 관리 등 일부 기능을 제외한 Warm Storage는 더 저렴한 비용으로 이용할 수 있습니다.\
예를 들어, 자주 사용하지 않는 폴더 계층의 데이터를 모두 Warm Storage로 이동하여 장기 보관하면, Shared Box의 Storage를 효율적으로 활용할 수 있습니다.\
이 매뉴얼에서는 관리자 페이지에서 Shared Box의 폴더 속성을 표시하여 파일이 Warm Storage로 자동 이동되도록 설정하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* Warm Storage를 사용할 수 있다면 관리자 페이지에 Warm Storage 관리 메뉴가 표시됩니다. 또한 폴더 속성에 자동 이동 설정이 표시됩니다.
* 자동 이동 대상으로 설정할 수 있는 폴더는 Shared Box의 1단계부터 6단계까지의 폴더만 해당됩니다.
* 상위 폴더에 자동 이동이 설정되어 있는 경우, 하위 폴더에는 해당 자동 이동 설정이 그대로 적용됩니다. 자동 이동 설정이 상속된 하위 폴더의 폴더 속성에는 자동 이동 설정을 변경하는 버튼이 표시되지 않습니다. 또한 상위 폴더의 설정에 따라 자동 이동된 하위 폴더의 파일에도 고스트가 표시됩니다.
* 하위 폴더에 자동 이동이 설정되어 있는 경우에는 상위 폴더에서 자동 이동을 사용함으로 설정할 수 없기 때문에, 상위 폴더의 폴더 속성에도 자동 이동 설정 변경 버튼이 표시되지 않습니다.
*   자동 이동은 폴더 단위로 설정합니다.

    예를 들어 아래와 같은 구조의 Shared Box에서 폴더 C에 대해 Warm Storage의 폴더 A로 자동 이동을 설정하면, Warm Storage 폴더 A 안에 폴더 C 이하의 폴더들이 기존 계층 구조를 그대로 유지한 상태로 생성되고, 폴더 C 이하의 파일들이 해당 위치로 이동됩니다.

<p align="center"><img src="../../.gitbook/assets/image (2265).png" alt=""></p>

* 파일이 Warm Storage로 자동 이동되면, '로그 현황' > '파일 이용 내역' 메뉴에 '자동 이동' 로그가 기록됩니다. 파일이 자동 이동될 때 폴더가 생성된 로그는 기록되지 않습니다.\
  자동 이동 로그를 확인하는 방법에 대해서는, [사용자의 파일 이용 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/log/file_usage_history)을 참조해 주십시오.
* 파일의 자동 이동 대상 위치에 동일한 이름의 폴더가 이미 있는 경우, 해당 폴더로 자동 이동됩니다.
* 자동 이동의 원본 폴더 이름이 변경된 경우, 자동 이동이 실행될 때 변경된 이름으로 Warm Storage에 새로운 폴더가 생성되며, 폴더 및 파일이 자동으로 이동됩니다.
* 자동 이동 대상 폴더에 동일한 이름의 파일이 있는 경우, 파일 이름 끝에 숫자가 추가됩니다. 원본 위치에 남는 고스트의 파일 이름 끝에도 동일한 숫자가 추가됩니다.
* 자동 이동 대상으로 설정된 Warm Storage 폴더의 이름이나 경로가 변경되면 자동 이동 설정의 이동 위치 정보도 함께 변경됩니다.
* 자동 이동 대상으로 설정된 Warm Storage 폴더가 삭제된 경우, 자동 이동이 실행될 때 자동으로 새 폴더가 생성됩니다.
* 파일이 자동으로 이동되면 다음 정보가 삭제됩니다.
  * Link History
  * 파일 잠금
  * 파일 유효기간
* 파일의 자동 이동 기준은 마지막 접속 일시입니다. 마지막 접속 일시의 다음 날을 기준일로 하며, 기준일을 포함해 이 매뉴얼의 절차에서 설정한 일수가 경과한 뒤 자정 0시부터 순차적으로 파일이 자동 이동됩니다.
* 다음 작업 중 하나라도 수행되어 대상 폴더에 저장된 파일에 접근이 발생하면, 해당 파일의 마지막 접속 일시가 갱신됩니다.
  * 업로드
  * 덮어쓰기 저장
  * 이름 변경
  * 이동
  * 자동 이동
  * 복사
  * 해동(Cold Storage)
  * 이전 버전 복원
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
    이 작업들에 대한 로그는 '로그 현황' > '파일 이용 내역' 메뉴의 '동작' 항목에서 확인할 수 있습니다.
* 사용자 페이지에서는 파일의 '파일 사용 이력' 화면에서 최종 접근 일시 및 조작 등의 이력을 확인할 수 있습니다.\
  자세한 내용은 [사용자 페이지에서 파일의 사용 이력을 확인하는 방법](https://help.directcloud.net/user_manual/file_management/file_log)을 참조해 주십시오.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**자동 이동 설정**
{% endhint %}

1. '공유설정' > ' Shared Box 관리'를 클릭하고 자동 이동을 설정할 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2266).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 '폴더 옵션' 설정을 표시하고 '자동 이동' 설정을 표시합니다.\
   자동 이동 설정이 없으면 '사용 안함'이 표시됩니다.\
   이미 자동 이동 설정이 되어 있으면 설정 내용이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2267).png" alt=""><figcaption></figcaption></figure>



3. 자동 이동 설정에서 수정 버튼을 클릭합니다. '자동 이동' 설정이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2268).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

4. 자동 이동의 '사용'을 선택하고 이동 위치 대상 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2270).png" alt=""><figcaption></figcaption></figure>



5. 파일을 이동할 폴더를 선택하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2271).png" alt=""><figcaption></figcaption></figure>



6. 파일의 마지막 접속 일시로부터 몇 일이 지난 후 자동 이동할지 드롭다운 목록에서 일수를 선택합니다. 10일부터 2000일까지의 값을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2272).png" alt=""><figcaption></figcaption></figure>



7. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2273).png" alt=""><figcaption></figcaption></figure>

설정한 내용이 표시됩니다.\
끝의 "i" 아이콘에 커서를 맞추면, 툴팁으로 이동처의 폴더를 확인할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2274).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**자동 이동 완료 이메일 확인**
{% endhint %}

자동 이동을 설정한 폴더의 파일이 자동 이동되면, 폴더에 접근 권한이 있는 모든 사용자에게 "000에서 자동이동이 진행되었습니다."라는 제목으로 메일이 전송됩니다.

<figure><img src="../../.gitbook/assets/image (2275).png" alt="" width="509"><figcaption></figcaption></figure>
