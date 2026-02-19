---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/file_management/wd_delete
---

# \[Web, Drive] 파일을 삭제하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 파일을 삭제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 파일을 삭제하는 사용자에게는 <마스터>, <전체권한>, <편집자>에 대한 접근 권한이 부여되어야 합니다.\
  <편집자> 접근 권한이 부여된 사용자는 자신이 업로드한 파일만 삭제할 수 있습니다.\
  자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission), [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/d_permission)을 참고해 주시기 바랍니다.
* 여러 폴더 파일에 체크가 있으면 위에서부터 순서대로 삭제가 수행됩니다.
* 파일을 한 번에 삭제할 때 삭제할 수 있는 파일 수에는 제한이 없습니다.
* 삭제 상태 화면에는 세션 시간이 없으므로 처리 시간이 초과되어 시간이 초과되지 않습니다.
* 삭제를 처리하는 동안 상태 화면에서 "×"를 클릭하거나 네트워크에 오류가 발생하면 "복사/이동 중 타임아웃이 발생하여 더 이상 진행할 수 없습니다."라는 오류 메시지가 표시됩니다.\
  이 때 오류 메시지가 표시되기 전에 처리 된 파일은 삭제되지만 처리 대기 상태의 파일은 삭제되지 않습니다.
*   삭제한 파일은 저장된 위치에 따라 삭제한 사용자의 휴지통 탭으로 이동합니다.

    * 'My Box' 및 'Shared Box' 파일: 사용자 휴지통의 'My Box/Shared Box' 탭으로 이동
    * DLP 폴더, Connect 폴더, Warm Storage지 및 Cold Storage 파일:\
      DLP, 연결, Warm Storage 및 Cold Storage 탭으로 이동합니다.

    그러나 사용자 휴지통의 탭 이름은 사용 가능한 옵션에 따라 달라집니다.
* 사용자의 휴지통이 사용 안 함으로 설정된 경우 삭제된 폴더 파일은 관리자의 휴지통으로 이동하지 않고 영구적으로 삭제됩니다.
* Web 브라우저 및 모바일 애플리케이션의 경우, 'DirectCloud AI'가 활성화된 폴더에서는 벡터 데이터 생성 중인 파일은 삭제할 수 없지만, 벡터화된 파일은 삭제할 수 있습니다.\
  DirectCloud 드라이브의 경우, 'DirectCloud AI'가 활성화된 폴더에서는 벡터 데이터 생성 중인 파일과 벡터화된 파일 모두 삭제할 수 없습니다.
* 사용자의 휴지통에 저장된 파일을 삭제하면 관리자의 휴지통으로 이동합니다.
* 관리자 페이지에서 '용량 관리' > '스토리지 현황' 메뉴에서 사용자의 휴지통에 저장된 파일을 확인할 수 있습니다.
* 사용자의 휴지통을 사용하도록 설정하면 Web 브라우저에서 폴더 파일을 삭제할 때 확인 화면이 표시되지 않습니다.
* DirectCloud의 옵션인 "DirectCloud-SHIELD DLP"를 계약한 경우, 사용자 페이지에 "DLP" 메뉴가, 사용자 휴지통에 "DLP" 탭이 표시됩니다.
* DirectCloud의 옵션인 "DirectCloud-CONNECT"를 이용할 수 있는 경우, 사용자 페이지에 "Connect" 메뉴가, 사용자 휴지통에 "Connect" 탭이 표시됩니다.
* Warm Storage를 이용할 수 있는 경우 사용자 페이지에 "Warm Storage" 메뉴가, 사용자 휴지통에 "Warm Storage" 탭이 표시됩니다.
* "Cold Storage"를 계약한 경우, 사용자 페이지에 "Cold Storage" 메뉴가, 사용자 휴지통에 "Cold Storage" 탭이 표시됩니다.
* Cold Storage에는 삭제 제한이 있기 때문에, 업로드, 이동, 자동 이동된 후 90일 동안은 파일을 삭제할 수 없습니다. 90일이 지나지 않은 경우, 이 매뉴얼 에서는 파일을 삭제하려 해도 "삭제" 작업을 선택할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 파일 삭제**
{% endhint %}

1. 삭제할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1453).png" alt=""><figcaption></figcaption></figure>

❶ 삭제할 파일을 체크하고 상단의 '삭제' 버튼을 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1454).png" alt=""><figcaption></figcaption></figure>

❷ 삭제하고자 하는 파일을 체크하고 마우스 오른쪽 버튼을 클릭하여 표시된 메뉴에서 \[삭제]를 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1455).png" alt=""><figcaption></figcaption></figure>

❸ 삭제할 파일의 오른쪽에 있는 ▼ 버튼을 클릭하고 표시된 메뉴에서 삭제를 클릭합니다. 여러 파일을 선택할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (1456).png" alt=""><figcaption></figcaption></figure>

사용자의 휴지통이 사용 안 함으로 설정된 경우 삭제 확인 화면이 표시되므로 \[확인] 버튼을 클릭합니다.

삭제가 시작되고 상태 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1457).png" alt=""><figcaption></figcaption></figure>



2. 삭제가 완료되었는지 확인합니다. 취소 버튼을 클릭하면 삭제를 취소할 수 있습니다.



{% hint style="warning" %}
**DirectCloud 드라이브에서 파일 삭제**
{% endhint %}

1. 삭제할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1458).png" alt=""><figcaption></figcaption></figure>



2. 삭제할 파일을 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 삭제를 클릭합니다.\
   여러 파일을 선택하여 삭제할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1459).png" alt=""><figcaption></figcaption></figure>

파일 삭제 화면이 표시됩니다.



3. '예'를 클릭하면 파일이 삭제됩니다.
