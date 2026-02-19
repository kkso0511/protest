---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/cold-storage/restoration
---

# Cold Storage의 파일을 복원하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 My Box나 Shared Box 등에서 사용되는 Hot Storage, 장기간 데이터 보존 시 사용하지 않는 일부 기능을 Hot Storage에서 제외하여 저비용화를 실현한 Warm Storage 외에 Cold Storage를 제공합니다.\
Cold Storage는 Warm Storage보다 장기 보존에 특화된 Storage입니다. 기능이나 데이터 복원에 관한 제한 사항이 있지만, Warm Storage와 비교했을 때 더 저렴한 비용으로 이용할 수 있습니다.\
이 매뉴얼에서는 Cold Storage에 저장된 파일을 Shared Box로 복원하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Cold Storage에서 파일을 복원하는 사용자는 복원 대상 폴더에 <마스터>, <전체권한> 접근 권한이 부여되어 있어야 합니다.
* Warm Storage를 이용할 수 있는 경우, 사용자 페이지에 ‘Warm Storage’ 메뉴가 표시됩니다.
* Cold Storage를 계약한 경우에는 사용자 페이지에 ‘Cold Storage’ 메뉴가 표시됩니다.
* Cold Storage에서는 월간 기준으로 1TB당 1,000개를 초과하는 파일을 복원할 수 없습니다. 월간 복원 가능 파일 수는 매월 1일에 초기화됩니다.
* 한 번에 복원 요청할 수 있는 최대 파일 수는 300개까지이며, 버전 이력의 개수도 파일 수에 포함된다는 점에 유의하십시오.
* Cold Storage에서 Shared Box로의 복원은 일반적으로 몇 분에서 최대 12시간 이내에 완료됩니다.
* 복원 대상 Shared Box 폴더로는 DirectCloud AI가 활성화된 폴더를 지정할 수 없습니다.
* ‘월간 복원 가능 파일 수’는 사용자 페이지에서 ‘Cold Storage’ 메뉴를 클릭하면 표시되는 사이드 메뉴에서 확인할 수 있습니다.
* Cold Storage로 업로드, 이동 또는 자동 이동된 파일에는 최소 보존 기간이 설정되어 있으므로, 최소 90일 동안은 삭제할 수 없습니다.
* 복원 요청은 취소할 수 없습니다.
* 복원 대상 Shared Box 폴더에 동일한 이름의 파일이 있는 경우, 파일 이름 끝에 숫자가 자동으로 추가되어 별도의 파일로 복원됩니다.
* 복원 요청 후 지정된 Shared Box 폴더가 삭제된 경우, 자동으로 폴더가 생성된 뒤 파일이 복원됩니다.
* Cold Storage로의 자동 이동 및 Cold Storage에서의 복원과 관련된 로그는 파일의 ‘파일 사용 이력’ 화면에 다음과 같이 기록됩니다.
  * 파일이 Cold Storage로 자동 이동된 경우: ‘자동 이동’
  * Cold Storage에서 Shared Box로 파일을 복원한 경우: ‘해동’
*   Cold Storage로 이동 또는 자동 이동될 때 삭제된 다음 정보는 파일을 복원하더라도 복구되지 않습니다.

    * Link History
    * 파일 잠금
    * 파일 만료일
    * 즐겨찾기 정보
    * 전체 검색 데이터

    다음 정보는 유지됩니다.

    * 태그
    * 버전 이력
    * 코멘트
    * 파일 사용 이력
    * DirectCloud-SHIELD IRM으로 암호화된 파일

***

### 절차

{% hint style="warning" %}
**Cold Storage에서 파일 복원을 요청하기**
{% endhint %}

1. 복원하려는 파일이 저장된 Cold Storage의 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (362).png" alt=""><figcaption></figcaption></figure>



2. 다음 중 하나의 방법으로 파일을 복원할 수 있습니다.

❶ 복원하려는 파일을 체크한 후, 상단에 있는 ‘해동’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (363).png" alt=""><figcaption></figcaption></figure>

❷ 복원하려는 파일을 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 ‘해동’을 선택합니다.

<figure><img src="../../.gitbook/assets/image (365).png" alt=""><figcaption></figcaption></figure>

❸ 복원하려는 파일의 오른쪽에 있는 ▼ 버튼을 클릭하고, 표시된 메뉴에서 ‘해동’을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (366).png" alt=""><figcaption></figcaption></figure>

&#x20;      ‘해동’ 화면이 표시됩니다.



3. 복원 대상 Shared Box 폴더를 선택하고 ‘해동 요청’ 버튼을 클릭합니다.\
   **NOTE:** ‘새 폴더’를 클릭하면 새 폴더를 생성할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (367).png" alt=""><figcaption></figcaption></figure>

복원이 요청된 파일의 아이콘 오른쪽 아래에는 배지가 표시되며, 파일은 조작할 수 없게 됩니다.

<figure><img src="../../.gitbook/assets/image (368).png" alt=""><figcaption></figcaption></figure>

또한 복원 원본 폴더에 접근 권한이 있는 모든 사용자에게 ‘Cold Storage 파일 해동이 요청되었습니다.’라는 제목의 메일이 발송됩니다.



{% hint style="warning" %}
**복원 완료 메일 확인하기**
{% endhint %}

복원 요청한 파일의 복원이 완료되면, 복원 원본 폴더에 접근 권한이 있는 모든 사용자에게 ‘Cold Storage 파일 해동이 완료되었습니다.’라는 제목의 메일이 발송됩니다.

<figure><img src="../../.gitbook/assets/image (360).png" alt="" width="563"><figcaption></figcaption></figure>
