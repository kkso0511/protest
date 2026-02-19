---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_management/restoration
---

# 파일을 이전 저장 버전으로 복원하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 파일을 이전 버전으로 되돌리는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 Shared Box의 조작 방법을 설명하고 있지만, Connect 폴더와 DLP 폴더에서도 동일한 절차로 조작할 수 있습니다.
* 버전 관리 기능을 사용하려면 다음 설정을 완료해야 합니다.
  * 관리 페이지에서 '용량 관리' -> '스토리지 현황' 의 파일 버전 설정이 '사용'으로 설정되어야 합니다.
  * 폴더 속성 설정의 '버전 관리'가 '사용'으로 설정되어야 합니다.
* 파일을 이전 버전으로 되돌리려면 <마스터>, <전체권한>의 접근 권한이 부여되어야 합니다.
* 이전 버전에서 새 버전으로 파일을 복원할 수도 있습니다.
* 날짜를 지정하여 버전을 복원할 수 없습니다.
* 업데이트된 파일의 차이는 보존되지 않으며, 과거의 버전 파일이 일정 기간 동안 저장됩니다.
* 이전 버전 파일은 스토리지의 [계약 용량과 사용 용량을 확인하는 방법](https://help.directcloud.net/admin_manual/storage/check_capacity)으로 확인할 수 있습니다.
* [같은 이름의 파일 업로드 시 처리 기준 설정 방법](https://help.directcloud.net/admin_manual/upload/same_name_file)이 파일 덮어쓰기 설정으로 되어 있는 경우, 동일한 이름의 파일을 업로드하면 파일의 버전이 갱신됩니다.
* 파일을 다운로드하지 않고 온라인 편집하는 방법으로 다음을 수행하면 파일 버전이 업데이트됩니다.
  * 온라인 편집 화면에서 마우스 오른쪽 버튼을 클릭하고 표시된 메뉴에서 '코멘트 추가'를 선택합니다.
  * 온라인 편집 화면의 오른쪽 상단에있는 × 버튼을 클릭하고 확인 화면에서 "확인"버튼을 클릭하십시오.
* DirectCloud의 옵션인 "DirectCloud-CONNECT"를 이용할 수 있는 경우 "Connect" 메뉴가 표시됩니다.
* DirectCloud의 옵션인 "DirectCloud-SHIELD DLP"를 계약한 경우 "DLP" 메뉴가 표시됩니다.
* 다음 폴더에 저장된 파일은 업로드나 온라인 편집 등으로 갱신되지 않기 때문에, 버전 이력을 사용할 수 없습니다.
  * 'DirectCloud AI'가 활성화된 폴더
* Warm Storage를 이용할 수 있는 경우, 사용자 페이지에 "Warm Storage" 메뉴가 표시됩니다.
* Warm Storage의 파일이 덮어쓰기 저장된 경우에도, 버전 이력은 남습니다.\
  파일 프리뷰 기능을 사용할 수 있는 경우, Warm Storage에서 버전 이력을 확인할 수 있지만, 과거 버전 파일로 복원할 수는 없습니다.
* Cold Storage를 계약한 경우, 사용자 페이지에 "Cold Storage" 메뉴가 표시됩니다.
* Cold Storage에서는 버전 이력을 확인하거나 복원할 수 없습니다.
* Warm Storage 및 Cold Storage로 이동된 파일의 버전 이력은 삭제되지 않고 유지됩니다. 이동이나 복원 등의 작업으로 파일을 Shared Box로 되돌리면, 이전 버전으로 복원할 수 있습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 파일 버전을 복원**
{% endhint %}

1. 버전을 복원하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1343).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나로 파일 버전을 되돌립니다.

❶ 버전을 되돌리려는 파일을 체크하고 상단의 '버전 이력' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1344).png" alt=""><figcaption></figcaption></figure>

❷ 버전을 되돌리려는 파일을 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 "버전 이력"을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1345).png" alt=""><figcaption></figcaption></figure>

❸ 버전을 되돌리려는 파일의 오른쪽에 있는 ▼ 버튼을 클릭하고 표시된 메뉴에서 '버전 이력'을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1346).png" alt=""><figcaption></figcaption></figure>

버전 기록 화면에 최신 버전의 파일이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1347).png" alt=""><figcaption></figcaption></figure>



3. 왼쪽 영역에서 버전을 클릭하여 반환하려는 파일 버전을 표시합니다.

<figure><img src="../../.gitbook/assets/image (1348).png" alt=""><figcaption></figcaption></figure>



4. 선택한 버전으로 파일을 되돌릴 수 있다면 복원 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1349).png" alt=""><figcaption></figcaption></figure>

파일이 복원됩니다.



5. 미리보기 등으로 파일을 보고 선택한 버전으로 파일이 복원되었는지 확인합니다.



{% hint style="warning" %}
**DirectCloud 드라이브에서 파일 버전 복원**
{% endhint %}

1. 버전을 복원하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1350).png" alt=""><figcaption></figcaption></figure>



2. 버전을 되돌리려는 파일을 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 'DirectCloud-Drive' > '버전이력'을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1351).png" alt=""><figcaption></figcaption></figure>

버전 기록과 최신 버전의 파일이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1352).png" alt=""><figcaption></figcaption></figure>



3. 왼쪽 영역에서 버전을 클릭하여 복원하려는 파일 버전을 표시합니다.

<figure><img src="../../.gitbook/assets/image (1353).png" alt=""><figcaption></figcaption></figure>



4. 선택한 버전으로 파일을 되돌릴 수 있다면 복원 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1354).png" alt=""><figcaption></figcaption></figure>

&#x20;     파일이 복원되고 메시지가 표시됩니다.



5. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1355).png" alt=""><figcaption></figcaption></figure>



6. 미리보기 등으로 파일을 보고 선택한 버전으로 파일이 복원되었는지 확인합니다.
