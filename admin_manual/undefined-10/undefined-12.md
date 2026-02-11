---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-10/undefined-12
---

# 관리자의 작업 내역을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, '로그 현황' > '관리자 페이지 변경 내역' 메뉴에서 관리자의 조작 이력을 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* '로그 현황' > '관리자 페이지 변경 내역' 메뉴에는 아래의 조작 이력이 기록됩니다.
  * 관리자 페이지에 계약 담당 관리자 또는 일반 관리자로 로그인하여 조작한 이력
  * PC용 Web 브라우저에 로그인하여, <마스터>로 설정된 폴더에서 슬라이드 화면의 접근 권한 및 폴더 속성을 설정한 이력
* 접근 권한 변경에 관한 조작 이력에서는 '누가 어떤 폴더의 권한을 변경했는지'는 확인할 수 있지만, '누구에게 어떤 권한을 설정했는지'는 확인할 수 없습니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 이용할 수 있는 경우, 관리자의 조작 이력에 Connect 폴더에 관한 조작 로그가 기록됩니다.
* DirectCloud의 옵션인 'DirectCloud-SHIELD DLP'를 계약한 경우, 관리자의 조작 이력에 DLP 폴더에 관한 조작 로그가 기록됩니다.
* Warm Storage를 이용할 수 있는 경우, 관리자의 조작 이력에 Warm Storage 폴더에 관한 조작 로그가 기록됩니다.
* Cold Storage를 계약한 경우, Cold Storage 폴더에 관한 조작 로그가 기록됩니다.
* Connect User를 초대한 쪽의 회사 ID 관리 페이지에서는, 초대받은 쪽의 관리자가 조작한 로그는 취득할 수 없습니다.
* Connect User를 초대받은 쪽의 회사 ID 관리 페이지에서는, Connect 폴더의 조작 로그를 취득할 수 없습니다.\
  단, [DirectCloud를 사용하는 다른 회사로부터의 Connect User 초대를 허용하는 방법](https://help.directcloud.net/admin_manual/undefined-6/directcloud-connect-user)에 따라 초대를 수락한 Connect User의 조작 이력은 취득할 수 있습니다.
* 계약 플랜이 '비즈니스' 이상인 경우, 로그의 보관 기간은 7년입니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**관리자 페이지 변경 내역 확인**
{% endhint %}

1. '로그 현황' > '관리자 페이지 변경 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1524).png" alt=""><figcaption></figcaption></figure>



2. '관리자 페이지 변경 내역' 에서 관리자의 작업 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (1525).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">항목</th><th>설명</th></tr></thead><tbody><tr><td>관리자</td><td>작한 관리자의 이름 및 사용자 ID가 표시됩니다.</td></tr><tr><td>구분</td><td>관리자가 실행한 조작이 표시됩니다.</td></tr><tr><td>로그</td><td>조작 이력의 상세 내용이 표시됩니다.<br>'드라이브 문자 할당 설정'의 로그인 경우, '▶' 버튼을 클릭하면 설정 내용이 표시됩니다.</td></tr><tr><td>위치</td><td><p>관리자가 조작한 장소로서, 아래 중 하나의 정보가 표시됩니다.</p><ul><li>Web：<br>PC Web 브라우저를 사용한 사용자 페이지에서의 조작</li><li>관리자 페이지：<br>관리자 페이지에서의 조작</li><li>API：<br>사용자 API, 관리자 API에 의한 조작</li></ul></td></tr><tr><td>날짜</td><td>관리자가 조작한 일시가 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**관리자 페이지 변경 내역을 필터링하여 표시**
{% endhint %}

관리자 작업 화면에서 관리자의 작업 내역을 기간, 사용자, 구분 및 건수로 필터링하여 볼 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1526).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>관리자의 조작 이력을 표시할 기간을, '최근 7일' '최근 15일' '최근 1개월' '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작일부터 현재까지의 관리자의 조작 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>클릭하여 드롭다운 리스트를 표시하고, 관리자의 조작 이력을 필터링하여 표시하고 싶은 구분을 선택합니다.</td></tr><tr><td>❹</td><td>조작 이력을 조작한 관리자로 필터링하려는 경우, '사용자명' 또는 '사용자 ID'를 입력합니다.</td></tr><tr><td>❺</td><td>관리자의 조작 이력을 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**관리자 페이지 변경 내역을 CSV 파일로 다운로드하기**
{% endhint %}

1. '관리자 페이지 변경 내역'에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.\
   관리자의 조작 이력은 대량의 데이터가 될 수 있으므로 미리 필터링하여 표시한 후 다운로드 하는 것이 좋습니다.

<figure><img src="../../.gitbook/assets/image (1527).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1528).png" alt=""><figcaption></figcaption></figure>
