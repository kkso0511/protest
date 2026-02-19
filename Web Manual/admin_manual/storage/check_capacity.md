---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/storage/check_capacity
---

# 계약 용량과 사용 용량을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는  '용량 관리' >  '스토리지 현황' 메뉴에서 DirectCloud의 계약 용량과 사용 용량, 그리고 기능별 사용 내역을 확인하는 방법에 대해 설명합니다.\
또한 버전 파일과 휴지통에 보관되어 있는 파일을 삭제하는 방법에 대해서도 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '용량 관리' 항목을 사용할 수 있습니다.
* 스토리지 용량은 [계약 정보를 확인하는 방법](https://help.directcloud.net/admin_manual/home_menu/check_contract)의 절차에 따라 스토리지의 계약 용량과 사용 용량을 확인할 수도 있습니다.
* 계약 담당 관리자는 [사용자 페이지에서 계약 용량과 사용량을 확인하는 방법](https://help.directcloud.net/user_manual/home_menu/check_storage)의 절차를 통해서도 확인할 수 있습니다.
* 스토리지 사용량은 매일 오전 0시에 실행되는 배치 처리로 순차적으로 계산되어 Storage 용량 메뉴에 반영됩니다.
* 버전 파일이나 휴지통 삭제를 요청한 경우 Storage 용량 메뉴에는 즉시 반영되지 않습니다. 삭제 작업은 오전 2시부터 순차적으로 실행되며, 다음 날 오전 0시에 스토리지 사용량이 다시 계산되는 시점에 반영됩니다.
* DLP와 같은 새로운 스토리지가 추가된 경우, 사용 용량이 계산되기 전까지는 원형 그래프가 표시되지 않고 사용량은 하루 한 번 집계되므로 다음 날 확인해 주십시오라는 메시지가 표시됩니다.
* DirectCloud-CONNECT를 사용할 수 있는 경우, Connect 폴더 항목이 표시됩니다.
* Hot Storage 사용량에는 Warm Storage, Cold Storage, DLP Storage의 사용량이 포함되지 않습니다.
* '스토리지 현황' 메뉴의 Hot Storage 사용량, Warm Storage 사용량, Cold Storage 사용량, DLP Storage 사용량에서 삭제한 버전 파일과 관리자 휴지통에 보관되어 있던 폴더 및 파일은 복원할 수 없습니다.
* DirectCloud AI가 활성화된 폴더에서 생성된 벡터 데이터는 사용 용량에 포함되지 않습니다.
* Warm Storage를 사용할 수 있는경우 Warm Storage 사용량이 표시됩니다.
* Cold Storage를 계약한 경우 Cold Storage 사용량이 표시됩니다.
* DirectCloud-SHIELD DLP를 계약한 경우 DLP Storage 사용량이 표시됩니다.
*   Hot Storage 사용량, Warm Storage 사용량, Cold Storage 사용량, DLP Storage 사용량의 관리자 휴지통에는 각각 My Box·Shared Box, Warm Storage, Cold Storage, DLP 폴더에서 삭제되어 관리자 휴지통으로 이동된 폴더와 파일의 용량이 합산됩니다.

    다만, 폴더와 파일 자체는 동일한 관리자 휴지통으로 이동됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Hot Storage 계약 용량 및 사용 용량 확인**
{% endhint %}

이 매뉴얼에서는 Hot Storage 사용량에 표시되는 정보를 확인하는 방법에 대해 설명합니다.

1. '용량 관리' > '스토리지 현황' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2094).png" alt=""><figcaption></figcaption></figure>



2. Hot Storage 사용량의 원형 차트를 참조하여 계약 용량과 사용 용량을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2096).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="93">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>사용 중인 스토리지의 용량과 사용률이 표시됩니다.</td></tr><tr><td>❷</td><td>계약하는 스토리지의 용량이 표시됩니다.</td></tr><tr><td>❸</td><td>스토리지 용량이 계산된 날짜와 시간이 표시됩니다.</td></tr></tbody></table>



3. Hot Storage  사용량의 오른쪽에 표시되는 기능별 사용 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2097).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="189">항목</th><th>내용</th></tr></thead><tbody><tr><td>My Box</td><td>My Box에 저장된 폴더 파일의 총 사용량이 표시됩니다.</td></tr><tr><td>Shared Box</td><td>Shared Box에 저장된 폴더 파일의 총 사용량이 표시됩니다.</td></tr><tr><td>Utility</td><td><p>다음 정보가 표시됩니다.</p><ul><li>My Box 내의 버전 파일<br>버전 관리 기능에 의해 My Box에 저장된 버전 파일의 총 용량이 표시됩니다.</li><li>Shared Box 내의 버전 파일<br>버전 관리 기능에 의해 Shared Box에 저장된 버전 파일의 총 용량이 표시됩니다.</li><li>사용자 휴지통<br>사용자 휴지통에 저장된 폴더와 파일의 총 사용량이 표시됩니다.</li><li>관리자 휴지통<br>My Box, Shared Box, 문서 관리 폴더, Connect 폴더에서 삭제되어 관리자 휴지통으로 이동한 폴더와 파일의 총 사용량이 표시됩니다.</li></ul></td></tr><tr><td>미 사용량</td><td>현재 여유 공간이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**Warm Storage 사용량의 계약 용량과 사용 용량을 확인하기**
{% endhint %}

이 매뉴얼에서는 Warm Storage 사용량에 표시되는 정보를 확인하는 방법에 대해 설명합니다.

1. '용량 관리' > '스토리지 현황' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2328).png" alt=""><figcaption></figcaption></figure>



2. Warm Storage 사용량의 원형 그래프를 확인하여 계약 용량과 사용 용량을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2329).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="77.199951171875">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>사용 중인 Warm Storage의 용량과 사용률이 표시됩니다.</td></tr><tr><td>2</td><td>계약된 Warm Storage 용량이 표시됩니다.</td></tr><tr><td>3</td><td>Warm Storage 용량이 계산된 날짜와 시간이 표시됩니다.</td></tr></tbody></table>



3. Warm Storage 사용량의 오른쪽에 표시된 기능별 사용 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2330).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="182.79998779296875">항목</th><th>내용</th></tr></thead><tbody><tr><td>Warm Storage</td><td>Warm Storage에 저장되어 있는 폴더와 파일의 총 사용량이 표시됩니다.</td></tr><tr><td>Utility</td><td><ul><li>Warm Storage 폴더 내의 버전 파일<br>버전 관리 기능에 의해 Warm Storage 폴더에 저장된 버전 파일의 총 용량이 표시됩니다.</li><li>사용자 휴지통<br>사용자 휴지통에 저장된 폴더·파일의 총 사용량이 표시됩니다.</li><li>관리자 휴지통<br>Warm Storage 폴더에서 삭제되어 관리자 휴지통으로 이동한 폴더·파일의 총 사용량이 표시됩니다.</li></ul></td></tr><tr><td>미 사용량</td><td>Warm Storage의 현재 사용 가능한 빈 용량이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**Cold Storage 사용량의 계약 용량과 사용 용량을 확인하기**
{% endhint %}

이 매뉴얼에서는 Cold Storage 사용량에 표시되는 정보를 확인하는 방법에 대해 설명합니다.

1. '용량관리' > '스토리지 현황' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2328).png" alt=""><figcaption></figcaption></figure>



2. Cold Storage의 원형 그래프를 확인하여 계약 용량과 사용 용량을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2331).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="77.199951171875">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>사용 중인 Cold Storage의 용량과 사용률이 표시됩니다.</td></tr><tr><td>2</td><td>계약된 Cold Storage 용량이 표시됩니다.</td></tr><tr><td>3</td><td>Cold Storage 용량이 계산된 날짜와 시간이 표시됩니다.</td></tr></tbody></table>



3. Cold Storage 사용량의 오른쪽에 표시된 기능별 사용 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2332).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="182.79998779296875">항목</th><th>내용</th></tr></thead><tbody><tr><td>Cold Storage</td><td>Cold Storage에 저장되어 있는 폴더와 파일의 총 사용량이 표시됩니다.</td></tr><tr><td>Utility</td><td><p>다음 정보가 표시됩니다.</p><ul><li><strong>Cold Storage 폴더 내의 버전 파일</strong><br>버전 관리 기능에 의해 Cold Storage 폴더에 저장된 버전 파일의 총 용량이 표시됩니다.</li><li><strong>사용자 휴지통</strong><br>사용자 휴지통에 저장된 폴더·파일의 총 사용량이 표시됩니다.</li><li><strong>관리자 휴지통</strong><br>Cold Storage 폴더에서 삭제되어 관리자 휴지통으로 이동한 폴더·파일의 총 사용량이 표시됩니다.</li></ul></td></tr><tr><td>미 사용량</td><td>Cold Storage의 현재 사용 가능한 빈 용량이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**버전 파일, 휴지통에 저장된 파일 삭제**
{% endhint %}

이 매뉴얼에서는, 'Hot Storage 사용량'에서의 조작 방법을 예로 설명하고 있지만, 'DLP Storage 사용량', 'Warm Storage 사용량'에 대해서도 동일한 절차로 조작할 수 있습니다.

1. '용량 관리' > '스토리지 현황' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2098).png" alt=""><figcaption></figcaption></figure>



2. Hot Storage 사용량의 Utility에서 용량을 비우려는 항목의 오른쪽에 표시되는 삭제 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2099).png" alt=""><figcaption></figcaption></figure>



3. 확인 화면에서 텍스트 상자에 DELETE를 입력하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2100).png" alt=""><figcaption></figcaption></figure>

화면 오른쪽 상단에 '삭제 요청이 완료되었습니다.'라는 메시지가 표시됩니다.\
회사 휴지통 삭제를 요청한 경우에는 삭제 요청 완료라고 표시됩니다. 자세한 사항은 이 다음 항목인 회사 휴지통을 삭제하고 싶은 경우를 참조해 주십시오.

**삭제 결과는 즉시 화면에 반영되지 않으며, 오전 0시에 스토리지 사용량이 다시 계산되는 시점에 반영됩니다.**

<figure><img src="../../.gitbook/assets/image (2101).png" alt=""><figcaption></figcaption></figure>

\
**\[회사 휴지통을 삭제하고 싶은 경우]**

관리자 휴지통 삭제를 요청한 경우에는 삭제 요청 완료라고 표시되며, 그 아래에 삭제 요청 완료 일시가 함께 표시됩니다.\
삭제 대상은 해당 일시에 관리자 휴지통에 존재하고 있던 폴더와 파일입니다.

<figure><img src="../../.gitbook/assets/image (2334).png" alt="" width="563"><figcaption></figcaption></figure>

다른 Utility와 동일하게, 삭제 작업은 오전 2시부터 순차적으로 실행됩니다.

다시 삭제 버튼을 클릭하면 삭제 요청 완료 일시가 갱신되며, 갱신된 해당 일시에 관리자 휴지통에 존재하고 있던 폴더와 파일이 삭제 대상으로 지정됩니다.
