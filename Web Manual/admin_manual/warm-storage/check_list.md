---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/warm-storage/check_list
---

# Warm Storage로 이동된 폴더 및 파일 정보를 목록에서 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 Shared Box에서 사용하는 Storage(Hot Storage) 외에 Warm Storage를 제공하고 있습니다. 일반적인 Hot Storage에서 링크나 버전 관리 등 일부 기능을 제외한 Warm Storage는 더 저렴하게 이용할 수 있기 때문에, 예를 들어 자주 사용하지 않는 데이터를 장기 보관하는 데 적합합니다.\
이 매뉴얼에서는 관리자 페이지에서 Shared Box에서 Warm Storage로 이동된 폴더 및 파일을 목록으로 표시하여 이동된 위치 정보를 확인하는 방법과, Warm Storage에 저장된 폴더 및 파일을 목록으로 표시하여 이동 전 위치 정보를 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정'을 사용할 수 있습니다.
* Warm Storage를 사용할 수 있다면 관리자 페이지에Warm Storage 관리 메뉴가 표시됩니다.
* Cold Storage를 이용 중인 경우에는 관리자 페이지에Cold Storage 관리 메뉴가 표시됩니다.
* Warm Storage와 Cold Storage에서는 링크를 생성할 수 없기 때문에, Warm Storage 및 Cold Storage의 파일 목록에는 Link History 정보가 표시되지 않습니다.
* Warm Storage의 파일을 Cold Storage로 이동하면 다음 파일 목록에 표시되던 아이콘이 사라지며, 파일 정보를 확인할 수 없게 됩니다.
  * Shared Box: 저장 위치 정보
  * Warm Storage: 이동 전 정보

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Shared Box의 폴더 및 파일 목록에서 대상 정보를 확인합니다.**
{% endhint %}

Shared Box의 폴더 및 파일 목록을 표시하여 Warm Storage로 이동된 폴더와 파일의 정보를 확인하는 방법을 설명합니다.

1. '공유 설정' > 'Shared Box' 메뉴를 클릭한 후, 폴더 트리에서 제1계층 이후의 폴더를 클릭합니다.\
   자세한 절차에 대해서는, [폴더에 저장된 폴더와 파일을 목록으로 표시하는 방법](https://help.directcloud.net/admin_manual/folder/file_list)의 '제2계층 이후의 폴더·파일 목록을 표시하기'를 참조해 주십시오.

<figure><img src="../../.gitbook/assets/image (351).png" alt=""><figcaption></figcaption></figure>



2. '사용현황' 설정의 항목 중 '파일 목록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (352).png" alt=""><figcaption></figcaption></figure>

선택한 폴더에 저장된 폴더와 파일이 목록으로 표시됩니다.\
Warm Storage로 이동된 폴더와 파일에는 저장 위치 정보 항목에 아이콘이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (354).png" alt=""><figcaption></figcaption></figure>



3. '연결 정보'에서 확인할 폴더 또는 파일 옆의 아이콘을 클릭합니다.\
   &#x20;Warm Storage로 이동된 폴더 또는 파일의 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (355).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="213.20001220703125">항목</th><th>설명</th></tr></thead><tbody><tr><td>보관 위치</td><td>폴더 및 파일을 저장할 폴더의 폴더 경로가 표시됩니다.</td></tr><tr><td>이동날짜</td><td>저장 위치로 이동한 날짜와 시간이 표시됩니다.</td></tr><tr><td>사용자 이름</td><td>폴더나 파일을 이동한 사용자 이름과 사용자 ID와 이동 방법("수동 이동" 또는 "자동 이동")이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**Warm Storage 폴더 및 파일 목록에서 원본 정보를 확인합니다.**
{% endhint %}

Warm Storage 폴더 및 파일 목록을 표시하고 이동할 정보를 확인하는 방법을 설명합니다.

1. '공유 설정' > 'Warm Storage 관리' 메뉴를 클릭한 후, 폴더 트리에서 제1계층 이후의 폴더를 선택합니다.

<figure><img src="../../.gitbook/assets/image (356).png" alt=""><figcaption></figcaption></figure>



2. '사용현황' 설정의 항목 중 '파일 목록' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (357).png" alt=""><figcaption></figcaption></figure>

선택한 폴더에 저장된 폴더와 파일이 목록에 표시됩니다.\
Shared Box에서 Warm Storage로 이동된 폴더 및 파일에는 '연결 정보' 항목에 아이콘이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (358).png" alt=""><figcaption></figcaption></figure>



3. '연결 정보' 에서 확인할 폴더 또는 파일 아이콘을 클릭합니다.\
   Shared Box에서 Warm Storage로 이동된 폴더 또는 파일 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="212.4000244140625">항목</th><th>설명</th></tr></thead><tbody><tr><td>위치</td><td>폴더나 파일을 이동할 폴더의 폴더 경로가 표시됩니다.<br>이동한 폴더나 파일이 더 이동되면 이동한 후의 폴더 경로가 표시됩니다.</td></tr><tr><td>이동날짜</td><td>파일 또는 폴더가 이동된 날짜와 시간이 표시됩니다.</td></tr><tr><td>사용자 이름</td><td>폴더나 파일을 이동한 사용자 이름과 사용자 ID와 이동 방법("수동 이동" 또는 "자동 이동")이 표시됩니다.</td></tr></tbody></table>
