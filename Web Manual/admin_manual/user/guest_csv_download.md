---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/user/guest_csv_download
---

# Guest 정보를 CSV 파일로 다운로드하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 ‘Guest' 관리 메뉴에서 관리자 페이지에 등록되어 있는 Guest 정보 목록을 CSV 파일로 일괄 다운로드하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* Guest 정보를 CSV 파일로 다운로드할 수 있는 최대 행 수는 100,000행입니다.
* CSV 다운로드는 여러 번 나누어서 요청할 수 있습니다. 하지만 다운로드 처리가 중단 없이 계속 진행되다가 총 3시간을 넘으면, 시스템에서 오류로 처리되어 다운로드가 실패합니다.
*   다운로드되는 CSV 파일의 문자 코드는 ‘환경 설정’ > ‘상세 설정’ 메뉴의 ‘문자 인코딩’ 설정에서 지정된 값이 적용됩니다.

    자세한 내용은 [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참고해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Guest 정보 다운로드 요청**
{% endhint %}

1. '계정 관리' > 'Guest' 메뉴를 선택하고 'Guest 관리' 탭을 선택한 다음 'Guest 일괄 등록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1758).png" alt=""><figcaption></figcaption></figure>



2. CSV 다운로드 화면을 표시하고 'Guest CSV 다운로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1759).png" alt=""><figcaption></figcaption></figure>



3. CSV 요청 확인 화면에서 출력 행 수와 문자 코드를 확인한 다음 '확인' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1761).png" alt=""><figcaption></figcaption></figure>

CSV 다운로드 처리가 완료되면 요청한 계약 담당 관리자 또는 일반 관리자의 이메일 주소로 알림 이메일을 받게 됩니다.



{% hint style="warning" %}
**이메일 링크에서 CSV 파일 다운로드**
{% endhint %}

1. 알림 이메일을 열고 '다운로드 바로가기' URL을 클릭합니다.\
   CSV 파일 다운로드 페이지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1762).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. Guest CSV 다운로드 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1763).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. CSV 파일을 열어 사용자 정보를 확인합니다.

<figure><img src="../../.gitbook/assets/image (1764).png" alt=""><figcaption></figcaption></figure>
