---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/trash/wd_user_trash
---

# \[Web, Drive] 사용자 휴지통의 폴더 및 파일을 확인, 조작하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 사용자 페이지에서 삭제되어 휴지통으로 이동한 폴더와 파일을 확인하고, 복구하거나 완전히 삭제하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 휴지통 기능을 사용하려면, 먼저 관리자 페이지 에서 사용자 휴지통을 활성화해야 합니다.
* DirectCloud의 옵션인 DirectCloud-CONNECT를 이용할 수 있는 경우에는 ‘Connect’ 메뉴가 표시되며, 사용자 휴지통에 ‘Connect’ 탭이 추가됩니다.
* DirectCloud-SHIELD DLP를 계약한 경우에는 ‘DLP’ 메뉴가 표시되며, 사용자 휴지통에 ‘DLP’ 탭이 추가됩니다.
* Warm Storage를 이용할 수 있는 경우, ‘Warm Storage’ 메뉴가 표시되며, 사용자 휴지통에도 ‘Warm Storage’ 탭이 추가됩니다.
* Cold Storage를 계약한 경우에는 ‘Cold Storage’ 메뉴가 표시되며, 사용자 휴지통에 ‘Cold Storage’ 탭이 추가됩니다.
* 이 매뉴얼에서는 DirectCloud-CONNECT, DirectCloud-SHIELD DLP, Warm Storage, Cold Storage를 사용할 수 있는 환경을 예로 들어 설명합니다.
* 사용자 휴지통의 보존 기간은 모든 탭에 공통으로 설정되며, ‘1일’, ‘3일’, ‘5일’, ‘7일’, ‘30일’, ‘제한 없음’ 중 하나로 지정할 수 있습니다.
* 사용자 휴지통에서는 폴더나 파일을 검색할 수 없습니다.
* 휴지통에 표시되는 폴더와 파일은 기본적으로 이름 기준 오름차순으로 정렬됩니다.\
  헤더 항목의 ‘이름’, ‘크기’, ‘갱신일시’, ‘종류’를 클릭하면 정렬 순서를 변경할 수 있습니다.
* 링크가 설정된 폴더나 파일이 휴지통으로 이동되면 링크 정보는 삭제되며, 한 번 삭제된 링크 정보는 복구할 수 없습니다.
* 휴지통에 이동된 폴더와 파일을 복구할 수 있는 사용자는 다음 접근 권한이 필요합니다.
  * 제1계층 폴더 복구: <마스터>
  * 제2계층 이하 폴더 복구: <마스터>, <전체권한>
  * 파일 복구: <마스터>, <전체권한>, <편집자>
* 삭제 이전에 폴더가 존재하는 경우, 복구 시 자동으로 해당 폴더로 복구됩니다.
* My Box에서 삭제된 파일을 복구하면, 하위 폴더가 비어 있더라도 폴더 경로가 자동 생성되어 파일이 복구됩니다.\
  Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage에서 삭제된 파일을 복구할 때는 상황에 따라 동작이 달라집니다.
  * 복구 대상 폴더가 제2계층 이하에 있고 해당 폴더가 삭제된 경우: 폴더 경로가 자동으로 생성되어 파일이 복구됩니다.
  * 복구 대상 폴더가 제1계층에 있고 해당 폴더가 삭제된 경우: 복구 위치를 선택하는 화면이 표시됩니다.
  * 복구 대상의 Shared, Connect 메뉴 아래에 폴더가 존재하지 않는 경우: 복구 위치를 선택하는 화면이 표시됩니다.
  * 복구 대상의 DLP 메뉴 아래에 폴더가 존재하지 않는 경우: “현재 이용 가능한 DLP 폴더가 없습니다.”라고 표시됩니다.
  * 복구 대상의 Warm Storage 메뉴 아래에 폴더가 존재하지 않는 경우에는 “현재 이용 가능한 Warm Storage 폴더가 없습니다.”라고 표시됩니다.
  * 복구 대상의 Cold Storage 메뉴 아래에 폴더가 존재하지 않는 경우에는 “현재 이용 가능한 Cold Storage 폴더가 없습니다.”라고 표시됩니다.
* 사용자 휴지통의 ‘My Box / Shared’, ‘Connect’, ‘DLP’, ‘Warm Storage’, ‘Cold Storage’ 탭에서 파일을 복구할 때, 해당 파일이 삭제되기 전에 저장되어 있던 폴더가 관리자 휴지통으로 이동한 뒤 관리자 휴지통에서도 삭제된 경우, 폴더 경로에 ‘복구 위치 분실’ 이라는 메시지가 표시됩니다.\
  이 경우의 복구 위치는 복구 조건에 따라 달라집니다.
* 사용자 휴지통에서 파일을 복구할 때, 복구 대상 폴더에 동일한 이름의 파일이 존재하면 ‘폴더 또는 파일 복구’ 화면이 표시됩니다.\
  이 화면에서 새 파일 이름을 입력하고 ‘복구’ 버튼을 클릭하면 변경된 이름으로 파일이 복구됩니다.
* 사용자 휴지통에서 여러 파일을 동시에 복구할 경우, 복구 대상의 제1계층 폴더가 삭제되어 있거나, 동일한 이름의 파일이 여러 개 저장되어 있는 경우에는 오류 메시지가 표시됩니다.\
  이럴 때는 복구 대상 폴더를 다시 생성하거나, 파일을 개별적으로 선택해 복구해야 합니다.
*   DirectCloud AI가 활성화된 폴더에서 휴지통의 파일을 복원할 때, 복원 대상 폴더에 저장된 파일이 아래의 상한을 초과하면 각각 오류 메시지가 표시됩니다.

    * DirectCloud AI에서 사용할 수 있는 파일 수의 상한
    * DirectCloud AI에서 사용할 수 있는 파일 총 용량의 상한

    DirectCloud AI의 제한 및 보충 사항에 대해서는 [DirectCloud AI를 활용하기 위한 파일을 준비하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/file_preparation)을 참조해주시기 바랍니다.
* 또한, DirectCloud AI가 활성화된 폴더에서 삭제되어 휴지통으로 이동된 파일을 복구하면, 벡터 데이터도 함께 복구됩니다.
* 사용자의 휴지통에서 삭제된 폴더와 파일은 '회사 휴지통'으로 이동합니다.\
  자세한 내용은 [회사 휴지통에 있는 폴더와 파일을 복원하는 방법](https://help.directcloud.net/admin_manual/storage/company_trash_restore)의 휴지통에서 복원할 때 이동 위치를 참조하십시오.
* Cold Storage에는 삭제 제한이 있으며, 90일의 제한 기간은 파일이 처음 Cold Storage로 업로드, 이동 또는 자동 이동된 날짜를 기준으로 계산됩니다.\
  휴지통에서 복원하더라도 삭제 제한 기간이 다시 90일로 초기화되지는 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 휴지통 폴더 또는 파일 확인**
{% endhint %}

**\[사용자의 휴지통 보기]**

1. 사용자 페이지에서 휴지통 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1028).png" alt=""><figcaption></figcaption></figure>

My Box와 Shared Box의 휴지통인 \[My Box/Shared Box] 탭이 선택된 상태로 휴지통이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1029).png" alt=""><figcaption></figcaption></figure>



**\[휴지통 폴더 또는 파일 복구]**

1. 휴지통에서 복구할 폴더나 파일이 들어 있는 탭을 표시합니다.<br>
2. 다음 방법 중 하나로 폴더와 파일을 복구합니다.

❶  복구할 폴더나 파일을 체크하고 상단의 '복구' 버튼을 클릭합니다.\
여러 폴더 또는 파일을 선택하여 복구할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1030).png" alt=""><figcaption></figcaption></figure>

❷  복구할 폴더나 파일을 마우스 오른쪽 버튼으로 클릭하고 되돌리기를 클릭합니다.\
여러 폴더 또는 파일을 선택하여 복구할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1031).png" alt=""><figcaption></figcaption></figure>

❸  복구할 폴더 또는 파일의 오른쪽에 있는 ▼ 버튼을 클릭한 다음 표시된 메뉴에서 복구를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1032).png" alt=""><figcaption></figcaption></figure>

폴더와 파일이 삭제되기 전에 저장된 폴더로 이동합니다.



**\[휴지통 폴더 또는 파일 삭제]**

이 방법으로 삭제한 휴지통 폴더나 파일은 회사 휴지통으로 이동합니다.

1. 휴지통에서 삭제할 폴더나 파일이 들어 있는 탭을 표시합니다.
2. 다음 방법 중 하나로 폴더와 파일을 삭제합니다.

❶  삭제할 폴더나 파일을 체크하고 상단의 "삭제" 버튼을 클릭합니다.\
여러 폴더 또는 파일을 선택하여 삭제할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1033).png" alt=""><figcaption></figcaption></figure>

❷ 삭제할 폴더나 파일을 마우스 오른쪽 버튼으로 클릭하고 삭제를 클릭합니다.\
여러 폴더 또는 파일을 선택하여 삭제할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1034).png" alt=""><figcaption></figcaption></figure>

❸ 삭제할 폴더나 파일의 오른쪽에 있는 ▼ 버튼을 클릭한 후 표시된 메뉴에서 삭제를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1035).png" alt=""><figcaption></figcaption></figure>

3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1036).png" alt=""><figcaption></figcaption></figure>

폴더 또는 파일이 삭제되고 회 휴지통으로 이동합니다.



**\[휴지통 폴더와 파일 모두 삭제]**

휴지통의 각 탭에 저장된 폴더와 파일을 한 번에 삭제할 수 있습니다.\
삭제한 휴지통 폴더나 파일은 회사사 휴지통으로 이동합니다.

1. 휴지통에서 삭제할 폴더나 파일이 들어 있는 탭을 표시합니다.
2. 상단의 휴지통 비우기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1037).png" alt=""><figcaption></figcaption></figure>

3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1038).png" alt=""><figcaption></figcaption></figure>

폴더와 파일이 모두 삭제됩니다.



{% hint style="warning" %}
**DirectCloud 드라이브에서 휴지통 폴더 또는 파일 확인**
{% endhint %}

아래 절차는 휴지통의 모든 탭에서 동일한 방식으로 수행할 수 있습니다.

**\[사용자의 휴지통 보기]**

1. 작업 트레이를 클릭하고 DirectCloud 드라이브 아이콘을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1039).png" alt=""><figcaption></figcaption></figure>

DirectCloud 드라이브 설정 화면이 표시됩니다.



2. 휴지통 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1040).png" alt=""><figcaption></figcaption></figure>

My Box와 Shared Box의 휴지통인 \[My Box/Shared Box] 탭이 선택된 상태로 휴지통이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1042).png" alt=""><figcaption></figcaption></figure>



**\[휴지통 폴더 또는 파일 복구]**

1. 휴지통에서 복구할 폴더나 파일이 들어 있는 탭을 표시합니다.
2. 다음 방법 중 하나로 폴더와 파일을 복구합니다.

❶  복구할 폴더나 파일을 체크하고 상단의 '복구' 버튼을 클릭합니다.\
여러 폴더 또는 파일을 선택하여 복구할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1043).png" alt=""><figcaption></figcaption></figure>

❷  복구할 폴더나 파일을 마우스 오른쪽 버튼으로 클릭하고 복구를 클릭합니다.\
여러 폴더 또는 파일을 선택하여 복구할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1044).png" alt=""><figcaption></figcaption></figure>

❸ 복구할 폴더 또는 파일의 오른쪽에 있는 ▼ 버튼을 클릭한 다음 표시된 메뉴에서 되돌리기를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1045).png" alt=""><figcaption></figcaption></figure>

폴더와 파일이 삭제되기 전에 저장된 폴더로 이동합니다.



**\[휴지통 폴더 또는 파일 삭제]**

이 방법으로 삭제한 휴지통 폴더나 파일은 회사 휴지통으로 이동합니다.

1. 휴지통에서 삭제할 폴더나 파일이 들어 있는 탭을 표시합니다.
2. 다음 방법 중 하나로 폴더와 파일을 삭제합니다.

❶  삭제할 폴더나 파일을 체크하고 상단의 "삭제" 버튼을 클릭합니다.\
여러 폴더 또는 파일을 선택하여 삭제할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1046).png" alt=""><figcaption></figcaption></figure>

❷  삭제할 폴더나 파일을 마우스 오른쪽 버튼으로 클릭하고 삭제를 클릭합니다.\
여러 폴더 또는 파일을 선택하여 삭제할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1047).png" alt=""><figcaption></figcaption></figure>

❸  삭제할 폴더나 파일의 오른쪽에 있는 ▼ 버튼을 클릭한 후 표시된 메뉴에서 삭제를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1048).png" alt=""><figcaption></figcaption></figure>

3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1049).png" alt=""><figcaption></figcaption></figure>

폴더 또는 파일이 삭제되고 회사 휴지통으로 이동합니다.



**\[휴지통 폴더와 파일 모두 삭제]**

휴지통의 각 탭에 저장된 폴더와 파일을 한 번에 삭제할 수 있습니다.\
삭제한 휴지통 폴더나 파일은 회사 휴지통으로 이동합니다.

1. 휴지통에서 삭제할 폴더나 파일이 들어 있는 탭을 표시합니다.
2. 상단의 휴지통 비우기 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1050).png" alt=""><figcaption></figcaption></figure>

3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1051).png" alt=""><figcaption></figcaption></figure>

폴더와 파일이 모두 삭제됩니다.
