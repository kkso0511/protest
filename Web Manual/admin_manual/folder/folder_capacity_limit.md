---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/folder/folder_capacity_limit
---

# 폴더의 용량 제한을 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 폴더를 지정하여 해당 폴더에 저장할 수 있는 폴더와 파일의 용량을 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 환경 설정 메뉴의 Shared Box와 Connect 관리 메뉴에서의 설정 방법을 설명하고 있지만, Shared Box와 Connect 관리 이외의 메뉴에서도 동일한 절차로 설정할 수 있습니다.
* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '공유 설정' 메뉴를 사용할 수 있습니다.
* 최대 용량은 계약 플랜의 총 Storage 용량 내에서 설정할 수 있습니다.
* 1GB(기가바이트)는 1,024MB(메가바이트)로 환산됩니다.
* 초기 상태에서는 용량 제한이 '사용안함'으로 설정되어 있습니다.
* 용량 제한은 1단계 폴더에 설정하며, 설정 내용은 하위 폴더에 상속됩니다.
* DirectCloud AI를 활성화하면 폴더 속성에 DirectCloud AI가 표시됩니다.
* DirectCloud AI가 활성화된 폴더에 설정된 파일 총 용량 값이 본 매뉴얼의 절차로 설정한 용량 제한보다 작은 경우에는 DirectCloud AI의 용량 제한이 적용됩니다.
* DirectCloud-CONNECT를 사용할 수 있는 경우에는 Connect 관리 메뉴에서 Connect 폴더의 용량 제한을 설정할 수 있습니다.
* DirectCloud-SHIELD DLP를 계약하고 있는 경우에는 DLP 관리 메뉴에서 DLP 폴더의 용량 제한을 설정할 수 있습니다.
* Warm Storage를 사용할 수 있다면 Warm Storage 관리 메뉴에서 Warm Storage 폴더의 용량 제한을 설정할 수 있습니다.
* Cold Storage를 계약하고 있는 경우에는 Cold Storage 관리 메뉴에서 Cold Storage 폴더의 용량 제한을 설정할 수 있습니다.
* Cold Storage의 파일을 Shared Box로 복원하는 경우, 복원 대상 Shared Box의 용량 제한을 초과하고 있어도 복원이 실행됩니다.
* Warm Storage 또는 Cold Storage로 파일이 자동으로 이동된 경우에는 각 Storage 폴더의 용량 제한이 적용됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Shared Box의 용량 제한 설정**
{% endhint %}

1. '공유 설정' > 'Shared Box' 관리 메뉴를 선택하고 폴더 용량 한도를 변경하려는 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1939).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 폴더 속성 설정에서 용량 제한의 변경 버튼을 클릭합니다.\
   용량 제한 설정이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1940).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. 용량제한의 '사용'을 선택하고 사용 가능한 용량을 메가바이트 단위로 입력한 다음 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1941).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**용량 한도를 초과한 경우**
{% endhint %}

사용자가 폴더 파일을 업로드 할 때 제한된 용량을 초과하면 "할당 용량을 넘고 있기 때문에 파일을 추가할 수 없습니다."라는 오류 메시지가 표시됩니다.
