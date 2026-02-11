---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/undefined-11
---

# 외부로 반출된(다운로드된) 파일을 삭제하는 방법

### 개요

DirectCloud의 유료 옵션인 DireCtcloud-SHIELD IRM을 계약하신 경우, IRM(Information Rights Management)을 이용하여 의도치 않은 파일 유출을 방지할 수 있습니다. 다운로드나 공유 링크를 통해 외부로 반출된 암호화 파일은 DirectCloud-SHIELD IRM에서 관리되므로, 반출 문서 삭제 메뉴에서 삭제할 수 있습니다.\
이 매뉴얼 에서는 외부로 반출된 보안문서 파일을 삭제하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* 반출 문서 삭제 메뉴에서는 파일을 미리보기할 수 없습니다.
* 다운로드되는 CSV 파일의 문자 코드는 환경 설정 > 상세 설정 메뉴의 CSV 다운로드 시 문자 코드 설정에서 지정됩니다.\
  자세한 내용은 [다운로드하는CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/csv)을 참고해주시기 바랍니다.

### 절차

{% hint style="info" %}
**반출된 파일을 확인하기**
{% endhint %}

1. 'SHIELD' > '반출문서 삭제' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (216).png" alt=""><figcaption></figcaption></figure>

2. '반출문서 삭제'에서 반출된 파일 목록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (218).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="150">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일명/반출번호</td><td>파일의 이름과 32자리의 고유 식별 번호가 표시됩니다.<br>다운로드 또는 링크 전송을 통해 외부로 반출되는 파일에는 매번 고유 식별 번호가 부여됩니다.</td></tr><tr><td>보안등급</td><td>파일에 부여된 보안등급 라벨이 표시됩니다.</td></tr><tr><td>사용자</td><td>파일을 반출한 사용자의 이름이 표시됩니다.</td></tr><tr><td>날짜</td><td>파일이 반출된 날짜와 시간이 표시됩니다.</td></tr><tr><td>크기</td><td>파일의 용량이 표시됩니다.</td></tr></tbody></table>

{% hint style="info" %}
**반출된 파일을 삭제하기**
{% endhint %}

1. '반출문서 삭제'에서 삭제하려는 파일의 동작 열에 표시된 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (220).png" alt=""><figcaption></figcaption></figure>

2. 확인 화면에서 '확인' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (221).png" alt=""><figcaption></figcaption></figure>

반출된 파일이 삭제되면, 반출 문서 삭제의 날짜 및 시간 열에 삭제된 날짜와 시간이 추가되며, 작업 열에서는 삭제 버튼이 표시되지 않게 됩니다.

<figure><img src="../../.gitbook/assets/image (222).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**삭제된 반출 파일에 접근한 경우**
{% endhint %}

삭제된 반출 파일을 열려고 하면 아래와 같은 '문서를 강제로 삭제하였습니다.'라는 제목의 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2399).png" alt="" width="365"><figcaption></figcaption></figure>

{% hint style="info" %}
**반출된 파일 목록을 조건별로 필터링하여 표시하기**
{% endhint %}

'반출문서 삭제'에서는 반출된 파일 목록을 기간, 사용자, 파일명, 고유 번호, 건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (223).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="106.79998779296875">No.</th><th>항목</th></tr></thead><tbody><tr><td>1</td><td>계약 시작일부터 현재까지의 반출된 파일 목록을 표시할 기간을 직전 7일, 직전 15일, 직전 1개월, 직전 3개월 중에서 선택합니다.</td></tr><tr><td>2</td><td>계약 시작일부터 현재까지의 반출된 파일 목록을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 최대 12개월입니다.</td></tr><tr><td>3</td><td>반출된 파일 목록을 작업을 수행한 사용자, 파일명, 고유 번호로 필터링하려는 경우 사용자명 또는 사용자 ID, 파일명, 고유 번호를 입력합니다.</td></tr><tr><td>4</td><td>반출된 파일 목록을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>

{% hint style="info" %}
**반출된 파일 목록을 CSV 파일로 다운로드하기**
{% endhint %}

1. '반출문서 삭제'에서 CSV 다운로드 버튼을 클릭합니다.\
   필요한 경우, 반출된 파일 목록을 먼저 필터링한 뒤 다운로드하시는 것을 권장합니다.

<figure><img src="../../.gitbook/assets/image (224).png" alt=""><figcaption></figcaption></figure>

2. CSV 파일을 열어 문제가 없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (225).png" alt=""><figcaption></figcaption></figure>
