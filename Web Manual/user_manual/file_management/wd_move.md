---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_management/wd_move
---

# \[Web, Drive] 파일을 이동하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 파일을 다른 폴더로 이동하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 본 매뉴얼에서는Shared Box에서 작업하는 방법에 대해 설명하지만 Shared Box 외에도 비슷한 절차를 수행할 수 있습니다.
*   파일 이동 기능은 내부적으로 이동 대상 파일을 삭제한 후, 이동할 폴더로 업로드하는 방식으로 처리됩니다. 따라서 파일을 이동하려는 사용자는 이동 전 폴더와 이동 후 폴더 모두에서 아래의 접근 권한을 가지고 있어야 합니다.

    * 이동 전 폴더:\
      <마스터>, <전체권한>
    * 이동 후 폴더:\
      <마스터>, <전체권한>, <편집자>, <편집자－>, <프리뷰어＋>, <업로더>

    자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission), [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/d_permission)을 참고해 주시기 바랍니다.
* 이동 화면에서 대상 폴더에 새 폴더를 만들려면 마스터, 전체권한의 접근 권한이 부여되어야 합니다.
* 다음의 모든 조건에 해당하는 경우, DirectCloud 드라이브에서 파일을 이동할 수 없습니다.
  * [워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/workflow/enable_workflow)에서 워크플로우가 활성 상태로 설정되어 있음
  * [특정 폴더에서 워크플로우를 활성화하는 방법](https://help.directcloud.net/admin_manual/folder/enable_workflow)에서 원본 폴더 또는 대상 폴더의 워크플로우가 사용함으로 설정되어 있음
  * 다운로드 워크플로우 또는 업로드 워크플로우의 신청자로 설정되어 있음
* Warm Storage로의 이동을 지원하는 Hot Storage는 Shared Box만 해당됩니다.
* Warm Storage 관련 폴더 및 파일의 조작 방법은\
  [\[Web, Drive\] Warm Storage로 폴더 또는 파일을 이동하는 방법](https://help.directcloud.net/user_manual/file_management/wd_move_to_warm) 및 [사용자 페이지에서 Ghost(고스트) 파일을 조작하는 방법](https://help.directcloud.net/user_manual/file_management/ghostfile)을 참고해 주십시오.
*   Cold Storage에서는 아래 방향으로 폴더 및 파일을 이동할 수 있습니다.

    * Hot Storage     ➡️ Cold Storage\
      Cold Storage   ➡️ Cold Storage\
      Warm Storage ➡️ Cold Storage

    단, Cold Storage로의 이동을 지원하는 Hot Storage 역시 Shared Box만 해당됩니다.

    또한 Cold Storage에서 Hot Storage로 파일을 이동할 수는 없습니다.\
    Cold Storage에서는 이동이 아닌 Cold Storage에서 복원을 이용해야 합니다.

    Cold Storage의 파일을 Shared Box로 복원하는 작업에 대해서는 [Cold Storage의 파일을 복원하는 방법](https://help.directcloud.net/user_manual/cold-storage/restoration)을 참고해 주십시오.
* 여러 개의 폴더와 파일을 선택한 경우, 선택된 목록의 위에서부터 순서대로 이동이 실행됩니다.
* 이동 대상 폴더에 동일한 이름의 폴더 또는 파일이 있을 경우, 이동할 수 없습니다.
* 이미 링크가 생성된 파일을 복사하는 경우에는 링크 정보가 복사되지 않지만, 파일을 이동하는 경우에는 링크 정보가 유지됩니다.
* DirectCloud 드라이브에서 로컬 환경의 폴더로 파일을 이동하는 경우, 실제 이동이 아니라 복사로 처리됩니다.
* 다음 애플리케이션에서는 파일 이동 시 상태 화면이 표시됩니다.
  * PC 버전 Web 브라우저
  * iOS 애플리케이션
  * Android 애플리케이션
  * 모바일 버전 Web 브라우저
* 여러 폴더와 파일을 동시에 이동할 때, 한 번에 이동할 수 있는 하위 폴더의 총수는 10,000개입니다.\
  10,001개 이상의 하위 폴더를 포함한 상위 폴더를 이동하려고 하면\
  "복사 또는 이동 대상이 최대값(10,000개)을 초과하여 조작을 진행할 수 없습니다."\
  라는 오류 메시지가 표시되며, 이동 처리는 중단됩니다.
*   한 번에 이동할 수 있는 파일 수에는 제한이 없습니다.\
    하지만 대량의 폴더 및 파일을 이동하는 경우, 처리 부하로 인해 속도가 저하될 수 있으므로 DirectCloud에서는 한 번에 1,000개 이상의 폴더 및 파일을 이동하는 작업은 권장하지 않습니다.

    특히 다음과 같은 경우에는 더욱 주의가 필요합니다.

    * 수십만 개의 버전 정보를 가진 파일 또는 그러한 파일이 포함된 폴더를 이동하는 경우
    * Shared Box에서 My Box 등, 상위 메뉴 간 이동을 수행하는 경우
* DirectCloud 드라이브에서 대량의 폴더 및 파일을 이동하면, 이동 대상 폴더에 반영되기까지 시간이 걸려 폴더와 파일이 정상적으로 표시되지 않을 수 있습니다.\
  이때 다음 사항에 유의해 주십시오.
  * 이동 처리가 완료될 때까지 해당 폴더와 파일에 대한 조작을 하지 않기
  * 이동 대상 폴더에서 이동한 파일이 보이지 않을 경우, 몇 시간 후 다시 확인하기
  * 이동 대상 폴더에 파일이 존재하지 않는 경우, 이동 전 폴더에 파일이 남아 있는지 확인하고, 한 번에 이동하는 파일 수를 줄인 뒤 다시 이동하기
*   DirectCloud 드라이브에서 이동 대상 폴더에 동일한 이름의 파일을 이동할 때 "파일을 교체"를 선택하면, 교체된 파일은 버전 정보를 포함하여 완전히 삭제되며 휴지통으로 이동하지 않습니다.

    또한 이 경우 다음 기록에는 삭제가 남지 않고 이동만 기록됩니다.

    * 사용자 페이지: 파일의 파일 사용 이력
    * 관리자 페이지: '로그 현황' ＞ '파일 이용 내역'
*   이동 처리 중 상태 화면의 × 버튼을 클릭하거나, 세션 시간이 10분을 초과한 경우\
    "복사 또는 이동 중에 타임아웃이 발생하여 작업이 중단되었습니다."\
    라는 오류 메시지가 표시됩니다.

    이때 오류 메시지가 표시되기 전까지 처리된 폴더와 이동 대상 폴더에 저장된 폴더·파일은 이동되지만, 처리 대기 중이던 폴더·파일은 이동되지 않습니다.
* DirectCloud AI가 활성화된 폴더에서의 파일 이동 가능 범위는 아래와 같습니다.
  * DirectCloud AI가 활성화된 폴더로 파일을 이동할 수 있는 폴더:\
    My Box, Shared Box
  * DirectCloud AI가 활성화된 폴더에서 파일을 이동할 수 있는 폴더:\
    My Box, Shared Box, Warm Storage, Cold Storage
*   DirectCloud AI가 활성화된 폴더로 파일을 복사하거나 이동하는 경우, 벡터 데이터가 생성됩니다.\
    벡터 데이터 생성 시에는 파일 내 텍스트 용량 등에 따라 비용이 발생하므로 주의가 필요합니다.

    DirectCloud AI가 생성하는 벡터 데이터 관련 상세 내용은 [DirectCloud AI 사양 및 참고 사항](https://help.directcloud.net/admin_manual/directcloud-ai/specification)을 참고해 주십시오.
* 또한 DirectCloud AI가 활성화된 폴더에서는 벡터 데이터 생성 중인 파일을 이동할 수 없습니다.
*   벡터 데이터가 생성되어 AI 라벨이 부여된 파일을 아래와 같이 이동한 경우,\
    벡터 데이터는 일일 배치 처리에 의해 오전 2시에 삭제됩니다.\
    단, 오전 2시 이전에 원래 폴더로 되돌리면 벡터 데이터는 재사용됩니다.

    AI 라벨이 삭제되는 이동 조건:

    * Shared Box의 DirectCloud AI 설정이 비활성화된 폴더로 이동한 경우
    * Shared Box 이외의 메뉴로 이동한 경우
*   Cold Storage로 폴더와 파일을 이동하면 다음 정보가 삭제됩니다.

    * 폴더 접근 권한
    * 폴더 속성
    * Link History
    * 파일 잠금
    * 파일 만료 설정
    * 즐겨찾기 정보
    * 전체 검색 데이터

    다음 정보는 유지됩니다.

    * 태그
    * 버전 이력
    * 코멘트
    * 파일 사용 이력
    * DirectCloud-SHIELD IRM의 보안등급 라벨과 irm 확장자
* Warm Storage와 Cold Storage의 사양에 대해서는\
  [Warm Storage와 Cold Storage의 차이](https://help.directcloud.net/user_manual/specification/difference_warm_cold)를 참고해 주십시오.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 파일 이동**
{% endhint %}

**\[이동하려는 파일이 저장된 폴더 표시]**

1. 이동하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1437).png" alt=""><figcaption></figcaption></figure>

\
**\[조작 메뉴에서 파일 이동]**

1. 다음 방법 중 하나로 파일의 이동 화면을 표시합니다.

❶  이동하고자 하는 파일을 체크하고 상단의 '이동' 버튼을 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1438).png" alt=""><figcaption></figcaption></figure>

❷  이동하고자 하는 파일을 체크하고 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 \[이동]을 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1439).png" alt=""><figcaption></figcaption></figure>

❸  이동할 파일의 오른쪽에 있는 ▼ 버튼을 클릭한 다음 표시된 메뉴에서 이동을 클릭합니다. 여러 파일을 선택할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (1440).png" alt=""><figcaption></figcaption></figure>

이동 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1441).png" alt=""><figcaption></figcaption></figure>



2. 이동할 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1442).png" alt=""><figcaption></figcaption></figure>



3. 필요한 경우 새 폴더를 클릭하여 새 폴더를 만듭니다.

<figure><img src="../../.gitbook/assets/image (1443).png" alt=""><figcaption></figcaption></figure>



4. 이동 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1444).png" alt=""><figcaption></figcaption></figure>

이동이 시작되고 상태 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1445).png" alt=""><figcaption></figcaption></figure>



5. 이동이 완료되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1446).png" alt=""><figcaption></figcaption></figure>

취소 버튼을 클릭하면 이동을 취소할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1447).png" alt=""><figcaption></figcaption></figure>

\
**\[드래그 앤 드롭으로 파일 이동]**

1. 이동하려는 파일을 드래그하여 대상 폴더에 놓습니다.\
   여러 파일을 체크하고 드래그 앤 드롭할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1448).png" alt=""><figcaption></figcaption></figure>

이동이 시작되고 상태 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1449).png" alt=""><figcaption></figcaption></figure>



2. 이동이 완료되었는지 확인합니다.

취소 버튼을 클릭하면 이동을 취소할 수 있습니다.



{% hint style="warning" %}
**DirectCloud 드라이브에서 파일 이동**
{% endhint %}

1. 이동하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1450).png" alt=""><figcaption></figcaption></figure>



2. 이동하려는 파일을 드래그하여 대상 폴더에 놓습니다.\
   여러 파일을 선택하고 끌어서 놓을 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1451).png" alt=""><figcaption></figcaption></figure>



3. 파일이 이동되었는지 확인합니다.
