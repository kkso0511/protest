---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/change_security_level
---

# 파일의 보안등급을 변경하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약하고 있는 경우, IRM(Information Rights Management)을 이용하여 의도하지 않은 파일의 유출을 방지할 수 있습니다.\
이 매뉴얼 에서는, DirectCloud-SHIELD IRM에서 부여된 파일의 보안등급 라벨을 변경하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* 암호화 문서 목록에는 Shared Box에 저장되어 있는 파일이 표시됩니다.\
  반출된 파일의 목록을 확인하고 싶은 경우에는 [외부로 반출된(다운로드된) 파일의 이용 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/export_file_usage)을 참고해주시기 바랍니다.
* 사용자 페이지에서 파일의 보안등급을 변경하는 방법을 통해 보안등급을 변경할 수도 있습니다.
* 이 매뉴얼 및 사용자 페이지에서 파일의 보안등급을 변경하는 방법을 사용해도, 모든 보안등급 라벨을 해제하여 보안등급 없음으로 설정할 수는 없습니다.
* 외부로 반출될 때 [보안문서 설정을 관리자 페이지에서 해제하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/release_security_doc) 또는 [사용자 페이지에서 파일의 보안문서 설정을 해제하는 방법](https://help.directcloud.net/user_manual/file_management/irm_unlock)을 통해 암호화가 해제되어 보안등급 라벨이 표시되지 않게 된 파일은 암호화 문서 목록에도 표시되지 않게 됩니다.
* [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/security_criteria)에서 상태가 비활성으로 설정되어 보안등급 라벨이 보안등급 없음으로 변경된 파일은 암호화 문서 목록에 표시됩니다.
* 다운로드되는 CSV 파일의 문자 코드는 환경 설정 > 상세 설정 메뉴의 CSV 다운로드 시 문자 코드 설정에서 지정됩니다.\
  자세한 내용은 [다운로드하는CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참고해주시기 바랍니다.

### 절차

{% hint style="warning" %}
**보안등급 라벨이 부여된 파일을 확인하기**
{% endhint %}

1. 'SHIELD' > '보안문서 현황' 목록 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (235).png" alt=""><figcaption></figcaption></figure>

2. '보안문서 현황'에서 보안등급 라벨이 부여된 파일의 목록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (236).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="147.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일</td><td>보안등급 라벨이 부여된 파일의 이름이 표시됩니다.</td></tr><tr><td>보안등급</td><td>파일에 부여된 보안등급 라벨이 표시됩니다.</td></tr><tr><td>사용자</td><td>파일을 업로드한 사용자의 이름이 표시됩니다.</td></tr><tr><td>날짜</td><td>파일이 업로드된 일시가 표시됩니다.</td></tr><tr><td>크기</td><td>파일의 용량이 표시됩니다.</td></tr><tr><td>동작</td><td>버튼을 클릭하면 암호화 정보 화면에서 아래 작업을 수행할 수 있습니다.<br>· 파일의 보안등급 변경<br>· 파일 암호화 해제</td></tr></tbody></table>

{% hint style="warning" %}
**파일 보안등급 변경**
{% endhint %}

1. '보안문서 현황'에서 보안등급을 변경하려는 파일의 동작 열에 있는 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (237).png" alt=""><figcaption></figcaption></figure>

2. '지정사유'의 편집 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (238).png" alt=""><figcaption></figcaption></figure>

3. 문서 속성을 클릭하여 변경하려는 보안등급에 해당하는 문서 속성을 활성화, 혹은 비활성화 상태로 만든 후, 저장 버튼을 클릭합니다. (여기서는 속성을 비활성화 하여 보안등급을 변경해보겠습니다.)

<figure><img src="../../.gitbook/assets/image (241).png" alt=""><figcaption></figcaption></figure>

4. 파일명 아래에 표시된 보안등급 라벨이 변경된 것을 확인한 후, 완료 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (242).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**보안등급 라벨이 부여된 파일을 추려서 표시하기**
{% endhint %}

'보안문서 현황'에서는 보안등급 라벨이 부여된 파일을 기간, 사용자, 파일명, 저장 위치(Shared Box 또는 My Box), 보안등급 라벨, 건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (243).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="93.20001220703125">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>계약 시작부터 현재까지 업로드된 파일 중 보안등급 라벨이 부여된 파일을 표시할 기간을<br>직전 7일, 직전 15일, 직전 1개월, 직전 3개월 중에서 선택합니다.</td></tr><tr><td>2</td><td>계약 시작부터 현재까지 업로드된 파일 중 보안등급 라벨이 부여된 파일을 표시할 기간을 직접 지정합니다.<br>지정할 수 있는 기간은 최대 12개월입니다.</td></tr><tr><td>3</td><td>클릭하여 드롭다운 목록을 표시한 뒤, 파일을 필터링할 저장 위치(Shared Box 또는 My Box)와 보안등급 라벨에 체크합니다.</td></tr><tr><td>4</td><td>보안등급 라벨이 부여된 파일을 업로드한 사용자나 파일명으로 필터링하려는 경우<br>사용자명 또는 사용자 ID, 파일명을 입력합니다.</td></tr><tr><td>5</td><td>보안등급 라벨이 부여된 파일의 표시 건수를<br>10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>

{% hint style="warning" %}
**보안등급 라벨이 부여된 파일을 CSV 파일로 다운로드하기**
{% endhint %}

1. '보안문서 현황'에서 CSV 다운로드 버튼을 클릭합니다.\
   필요에 따라 파일의 보안등급 및 보안문서변경 이력을 필터링한 후 다운로드하시기를 권장합니다.

<figure><img src="../../.gitbook/assets/image (244).png" alt=""><figcaption></figcaption></figure>

2. CSV 파일을 열어 문제가 없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (245).png" alt=""><figcaption></figcaption></figure>
