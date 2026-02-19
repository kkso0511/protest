---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/log/permission_history
---

# 사용자가 설정한 접근 권한의 이력을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, '로그 현황' > '전체권한자 권한변경 내역' 메뉴에서 <전체권한>의 접근 권한이 부여된 사용자에 의해 설정된 폴더에 대한 접근 권한 설정 이력을 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* DirectCloud의 옵션인 'DirectCloud-CONNECT'를 이용할 수 있는 경우라도, Connect User에게는 '접근 권한 설정 확장'이 적용되지 않기 때문에, Connect User는 접근 권한을 설정할 수 없습니다.\
  또한 Guest에게도 '접근 권한 설정 확장'이 적용되지 않기 때문에, Guest는 접근 권한을 설정할 수 없습니다.\
  따라서 '로그 현황' > '전체권한자 권한변경 내역' 메뉴에는 Guest 및 Connect User에 의한 접근 권한 설정 이력이 기록되지 않습니다.
* [사용자 페이지에서도 폴더에 대한 접근 권한을 설정할 수 있도록 하는 방법](https://help.directcloud.net/admin_manual/folder/user_permission_setting)의 절차에서, '속성'의 '접근 권한 설정 확장'이 '사용 안함'으로 설정되어 있는 경우에는, 폴더의 접근 권한 설정 이력이 기록되지 않습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**전체권한자 권한변경 내역을 확인하기**
{% endhint %}

1. '로그 현황' > '전체권한자 권한변경 내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2561).png" alt=""><figcaption></figcaption></figure>



2. 소유자의 권한 설정에서 사용자의 액세스 권한 설정 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2562).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">항목</th><th>설명</th></tr></thead><tbody><tr><td>이름</td><td>폴더에 접근 권한을 설정한 사용자의 이름이 표시됩니다.</td></tr><tr><td>로그</td><td>폴더에 대한 접근 권한 설정 이력이 표시됩니다.<br>사용자에 의한 접근 권한 설정 이력에서는 '누가 어떤 폴더의 권한을 변경했는지'는 확인할 수 있지만, '누구에게 어떤 방식으로 변경했는지'는 확인할 수 없습니다.</td></tr><tr><td>날짜</td><td>폴더에 접근 권한이 설정된 일시가 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**전체권한자 권한변경 내역을 필터링하여 표시**
{% endhint %}

전체권한자 권한변경 내역 화면에서 사용자에 의한 접근 권한 설정 이력을 기간, 사용자, 표시건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2563).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>사용자에 의한 접근 권한 설정 이력을 표시할 기간을, '최근 7일' '최근 15일' '최근 1개월' '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작일부터 현재까지의 사용자에 의한 접근 권한 설정 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>사용자에 의한 접근 권한 설정 이력을 사용자로 필터링하려는 경우, '사용자명' 또는 '사용자 ID'를 입력합니다.</td></tr><tr><td>❹</td><td>사용자에 의한 접근 권한 설정 이력을 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**전체권한자 권한변경 내역을 CSV 파일로 다운로드하기**
{% endhint %}

1. '전체권한자 권한변경 내역' 설정에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.\
   필요한 경우 전체권한자 권한변경 내역을 필터링하여 다운로드하는 것이 좋습니다.

<figure><img src="../../.gitbook/assets/image (2564).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2565).png" alt=""><figcaption></figcaption></figure>
