---
metaLinks:
  alternates:
    - https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/log/link_info
---

# 사용자가 생성한 링크의 설정 정보를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '로그 현황' > '링크 현황' 메뉴에서 사용자가 만든 링크의 구성 정보를 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* '로그 현황' > '링크 현황' 메뉴에는 Guest, LDAP 연동 및 SAML 연동으로 취득한 사용자의 설정 이력도 기록됩니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 이용할 수 있는 경우라도, Connect 폴더에서는 공유 링크를 생성할 수 없기 때문에 Connect 폴더의 링크 설정 정보는 확인할 수 없습니다.
* 링크를 생성한 이력은 '파일의 조작' 로그에 기록됩니다.\
  자세한 내용은 [사용자의 파일 이용 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/log/file_usage_history)을 참조해 주십시오.
* 링크에 관한 조작의 상세 내용과 링크에 대한 접근 로그는 사용자가 조작한 링크의 이력을 확인하는 방법의 절차에 따라 확인할 수 있습니다.
* 계약 담당 관리자 또는 일반 관리자에 의해 삭제된 사용자는 '삭제된 사용자'로 표시됩니다.\
  '삭제된 사용자'로 표시되는 로그 메뉴에 대해서는 관리 페이지의 '로그 현황'에서 삭제한 사용자는 어떻게 표시됩니까?를 참조해 주십시오.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**링크 현황 확인**
{% endhint %}

1. '로그 현황' > '링크 현황' 메뉴를 클릭하십시오.

<figure><img src="../../.gitbook/assets/image (1505).png" alt=""><figcaption></figcaption></figure>



2. 링크 현황 설정에서 링크 정보를 확인합니다.

<figure><img src="../../.gitbook/assets/image (1506).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="152">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일/폴더명</td><td>링크가 생성된 파일 이름 또는 폴더 이름이 표시됩니다.</td></tr><tr><td>링크</td><td>아이콘을 클릭하면 다른 탭에서 링크 수신 화면이 표시됩니다.</td></tr><tr><td>사용자</td><td>링크를 만든 사용자의 이름이 표시됩니다.</td></tr><tr><td>생성일자</td><td>링크가 작성된 날짜와 시간이 표시됩니다.</td></tr><tr><td>크기</td><td>링크를 만든 파일의 용량이 표시됩니다.</td></tr><tr><td>상태</td><td><p>링크의 상태가 표시됩니다. 상태 유형은 다음과 같습니다.</p><ul><li>유효<br>링크 URL에 액세스할 수 있는 상태</li><li>만료<br>링크가 만료되어 URL에 액세스할 수 없는 상태</li><li>삭제<br>링크 작성자 또는 계약 담당 관리자 · 일반 관리자가 링크 URL을 삭제했기 때문에 URL에 액세스 할 수없는 상태</li></ul></td></tr><tr><td>수신방법</td><td><p>수신자가 링크 내의 파일에 대해 조작할 수 있는 범위가 표시됩니다.<br>접근 권한의 종류는 아래와 같습니다.</p><ul><li>미리보기<br>파일의 미리보기만 가능합니다.</li><li>다운로드<br>파일의 다운로드만 가능합니다.</li><li>미리보기/다운로드<br>파일의 미리보기와 다운로드가 가능합니다.</li></ul></td></tr><tr><td>업로드</td><td><p>링크에 업로드 기능을 사용할지 여부를 표시합니다.<br>사용하는 경우 다음 용량 제한 중 하나를 설정합니다.</p><ul><li>100MB까지</li><li>500MB까지</li><li>1GB까지</li><li>2GB까지</li><li>5GB까지</li><li>용량 제한 없음</li></ul></td></tr><tr><td>비밀번호</td><td>링크에 설정된 비밀번호가 표시됩니다.</td></tr><tr><td>동작</td><td>링크를 삭제하는 버튼이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**링크 현황을 필터링하여 표시**
{% endhint %}

필터설정을 사용하면 링크의 설정 정보를 기간, 사용자, 파일 이름 및 표시건수로 필터링할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1507).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>링크 현황을 표시할 기간을, '최근 7일' '최근 15일' '최근 1개월' '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작부터 현재까지 링크의 구성 정보를 표시하는 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>링크 설정 정보를 조작한 사용자 또는 파일 이름으로 필터링하려면 사용자 이름, 사용자 ID 또는 파일 이름을 입력합니다.</td></tr><tr><td>❹</td><td>링크의 설정 정보를 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**링크 현황을 CSV 파일로 다운로드**
{% endhint %}

1. 링크 현황에서 'CSV 다운로드' 버튼을 클릭합니다.\
   링크의 현황의 정보는 대량의 데이터가 될 가능성이 있기 때문에, 미리 필터링하여표시하고 나서 다운로드 하는 것을 추천합니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1508).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1509).png" alt=""><figcaption></figcaption></figure>
