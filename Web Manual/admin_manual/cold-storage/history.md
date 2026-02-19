---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/cold-storage/history
---

# Cold Storage의 파일을 해동한 이력을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼 에서는 '로그 현황'> '파일 해동 완료 내역'에서 사용자가 Cold Storage에서 파일을 해동한 이력을 확인하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '로그 현황'기능을 사용할 수 있습니다.
* Cold Storage에서 파일을 해동한 이력은 다운로드 할 수 없습니다.

### 절차

{% hint style="warning" %}
**Cold Storage에서의 해동 이력을 확인하기**
{% endhint %}

1. '로그 현황'> '파일 해동 완료 내역' 메뉴를 클릭 합니다.

<figure><img src="../../.gitbook/assets/image (2283).png" alt=""><figcaption></figcaption></figure>



2. '파일 해동 완료 내역' 설정 화면에서 Cold Storage 파일의 해동 이력을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2284).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="201.20001220703125">항목</th><th>설명</th></tr></thead><tbody><tr><td>해동 결과</td><td>사용자가 요청한 복원의 결과가 표시됩니다. 성공 또는 실패가 표시됩니다.<br>실패일 경우 실패 이유 항목에 버튼이 표시됩니다.</td></tr><tr><td>파일명</td><td><ul><li>해동 결과가 성공인 경우:<br>해동이 요청된 파일 이름, 해동 대상 Shared Box 경로, 해동 원본 폴더 경로가 표시됩니다.</li><li>해동 결과가 실패인 경우:<br>해동이 요청된 파일 이름과 해동 원본 폴더 경로가 표시됩니다.</li></ul></td></tr><tr><td>이름</td><td>해동을 요청한 사용자의 이름이 표시됩니다.<br>이름에 마우스 커서를 올리면 툴팁으로 사용자 ID를 확인할 수 있습니다.</td></tr><tr><td>해동요청날짜</td><td>사용자가 해동을 요청한 일시가 표시됩니다.</td></tr><tr><td>해동완료날짜</td><td>Shared Box로의 해동이 완료된 일시가 표시됩니다.</td></tr><tr><td>사용 수량</td><td>해동된 개수가 표시됩니다. 이 수에는 파일의 버전 수가 포함됩니다.<br>해에 실패한 경우 0으로 표시됩니다.</td></tr><tr><td>실패 사유</td><td><p>복원 결과가 실패인 경우 버튼이 표시됩니다.<br>이 버튼을 클릭하면 실패 이유를 확인할 수 있습니다.<br></p><p>복원이 실패하는 이유는 다음과 같습니다.</p><ul><li>파일 이름 끝에 숫자가 추가되는 등의 이유로, 복원 후 파일 이름이 190자를 초과한 경우</li><li>서버 내부 오류가 발생한 경우</li><li>복원 요청 이후, 복원 대상 Shared Box에 DirectCloud AI가 적용된 경우</li></ul></td></tr></tbody></table>



3. 필요에 따라 이번 달에 파일 해동에 사용할 수 있는 기본해당 수와 사용 수를 확인합니다.

<figure><img src="../../.gitbook/assets/image (2285).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**Cold Storage에서의 해동 이력을 조건에 맞춰 필터링하여 표시하기**
{% endhint %}

Cold Storage에서 해동한 이력을 기간, 사용자, 파일명, 복원 결과, 건수 기준으로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2286).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="98.60003662109375">No.</th><th>설명</th></tr></thead><tbody><tr><td>①</td><td>Cold Storage에서 해동 이력을 표시할 기간을 최근 7일, 최근 15일, 최근 1개월, 최근 3개월 중에서 선택합니다.</td></tr><tr><td>②</td><td>계약 시작일부터 현재까지의 Cold Storage 해동 이력을 표시할 기간을 지정합니다. 지정할 수 있는 기간은 최대 12개월입니다.</td></tr><tr><td>③</td><td>클릭하여 드롭다운 목록을 열고, 필터링할 해동 결과로 성공 또는 실패를 선택합니다.  기본값은 전체로 설정되어 있어 모든 해 결과가 검색 대상에 포함됩니다.</td></tr><tr><td>④</td><td>해동 요청 사용자나 해동 대상 파일명으로 필터링하려면 사용자명 또는 사용자 ID, 파일명을 입력합니다.</td></tr><tr><td>⑤</td><td>Cold Storage 해동 이력을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>
