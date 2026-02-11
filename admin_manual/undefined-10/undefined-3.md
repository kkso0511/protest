---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-10/undefined-3
---

# 사용자가 파일에 유효기간을 설정한 내역을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, '로그 현황' > '파일기한 설정 현황' 메뉴에서 사용자가 파일에 유효기간을 설정한 이력을 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* Guest, LDAP 연동 및 SAML 연동으로 취득한 사용자의 설정 이력도 기록됩니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 사용할 수 있는 경우라도, Connect User는 파일의 유효기간을 설정할 수 없기 때문에, Connect User가 파일 유효기간을 설정한 이력은 기록되지 않습니다.
* 파일의 유효기간에 의해 삭제된 이력은 '파일의 조작 '로그에 기록됩니다.\
  자세한 내용은 [사용자의 파일 이용 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/undefined-10/undefined-2)을 참조해 주십시오.
* 파일의 유효기간 설정을 해제하면, '로그 현황' > '파일기한 설정 현황' 메뉴에 표시되지 않게 됩니다.
* 파일의 유효기간 설정을 해제했을 때의 로그는 기록되지 않습니다.
* 파일의 유효기간에 의한 자동 삭제는 설정일의 다음 날을 기산일로 하며, 기산일을 포함해 지정한 기간이 경과한 이후의 다음 날 2시 0분 0초에 실행됩니다.
* 파일의 유효기간에 의해 삭제된 파일은 '회사 휴지통 '으로 이동합니다.\
  자세한 내용은 회사 휴지통으로 이동한 폴더·파일을 확인하는 방법을 참조해 주십시오.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**파일기한 설정 현황 확인**
{% endhint %}

1. '로그 현황' > '파일기한 설정 현황' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1500).png" alt=""><figcaption></figcaption></figure>



2. '파일기한 설정 현황' 설정에서 파일 기한 설정 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (1501).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="132">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일</td><td>파일 유효기간을 설정한 파일 및 폴더 경로가 표시됩니다.</td></tr><tr><td>사용자</td><td>파일 유효기간을 설정한 사용자의 이름이 표시됩니다.</td></tr><tr><td>접속 아이피</td><td><p>연결할 IP 주소와 <a href="https://help.directcloud.net/admin_manual/images-and-media/ip">사용자 페이지에 로그인할 수 있는 IP 주소를 제한하는 방법</a>으로 허용된 IP 주소인지 여부에 따라 다음 정보 중 하나가 표시됩니다.</p><ul><li>허용된 IP 주소의 경우:<br>사내</li><li>허용되지 않는 IP 주소의 경우:<br>사외</li></ul></td></tr><tr><td>설정일</td><td>파일 유효기간을 설정한 일시가 표시됩니다.</td></tr><tr><td>삭제 예정일</td><td>파일 유효기간에 의해 삭제 예정인 일시가 표시됩니다.</td></tr><tr><td>크기</td><td>파일의 용량이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**파일기한 설정 현황을 필터링하여 표시**
{% endhint %}

'파일기한 설정 현황' 화면에서는 파일 기한의 설정 이력을 기간, 사용자, 파일명, 표시건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1502).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>파일 유효기간 설정 이력을 표시할 기간을, '최근 7일' '최근 15일' '최근 1개월' '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작일부터 현재까지의 파일 유효기간 설정 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>파일 유효기간 설정 이력을 조작한 사용자 또는 파일명으로 필터링하려면, '사용자명' 또는 '사용자 ID' 또는 '파일명'을 입력합니다.</td></tr><tr><td>❹</td><td>파일 유효기간 설정 이력을 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**파일기한 설정 현황을 CSV 파일로 다운로드**
{% endhint %}

1. 파일기한 설정 현황에서 'CSV 다운로드' 버튼을 클릭합니다.\
   필요한 경우 파일 기한 설정 내역을 필터링하여 다운로드하는것이 좋습니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1503).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1504).png" alt=""><figcaption></figcaption></figure>
