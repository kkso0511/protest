---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/folder_management/wd_delete
---

# \[Web, Drive] 폴더를 삭제하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 폴더를 삭제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 1계층 폴더를 삭제하는 사용자에게는 <마스터> 접근 권한이 부여되어 있어야 합니다.\
  자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission), [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/d_permission)을 참조하십시오.
* 2계층 이하 폴더를 삭제하는 사용자에게는 <마스터>, <전체권한> 접근 권한이 부여되어 있어야 합니다.
* DirectCloud 드라이브에서는 1계층 폴더를 삭제할 수 없습니다.
* Web 브라우저에서는 다음 방법으로 1계층 폴더를 삭제할 수 없습니다.
  * 오른쪽 클릭 메뉴에서 삭제 선택
  * 폴더 오른쪽의 ▼ 버튼을 눌러 표시되는 메뉴에서 삭제 선택
*   1계층 폴더를 삭제한 후 표시되는 "삭제되었사용자의 휴지통이 활성화되어 있는 경우, 삭제된 폴더는 저장되어 있던 위치에 따라 삭제한 사용자의 휴지통 탭으로 이동합니다.

    * My Box 및 Shared Box의 파일:\
      My Box / Shared 탭으로 이동
    * DLP 폴더, Connect 폴더, Warm Storage, Cold Storage의 파일:\
      DLP, Connect, Warm Storage, Cold Storage 탭으로 이동

    단, 사용자 휴지통의 탭은 이용 가능한 옵션에 따라 표시됩니다.

    또한 Web 브라우저에서 폴더·파일을 삭제할 때는 확인 화면이 표시되지 않습니다.
* 삭제 권한이 부여된 경우, 접근 권한을 갖지 않은 하위 폴더를 포함한 부모 폴더도 삭제할 수 있습니다.
* 폴더를 한 번에 삭제할 때 삭제할 수 있는 폴더 수에는 제한이 없습니다.
* 삭제 상태 화면에는 세션 시간이 없기 때문에, 처리 시간이 길어져도 타임아웃이 발생하지 않습니다.
*   삭제 처리 중 상태 화면의 × 버튼을 누르거나 네트워크 오류가 발생한 경우에는\
    “삭제 중 타임아웃이 발생하여 더 이상 진행할 수 없습니다.”\
    라는 오류 메시지가 표시됩니다.

    이 경우 오류 메시지가 표시되기 전까지 처리된 폴더와 해당 폴더의 직속 하위 폴더는 삭제되지만, 처리 대기 중인 폴더는 삭제되지 않습니다.
* 사용자 휴지통이 비활성화되어 있는 경우, 삭제된 폴더·파일은 관리자의 휴지통으로 이동하지 않고 완전히 삭제됩니다.
* 사용자 휴지통에 저장되어 있는 폴더를 삭제하면 관리자 휴지통으로 이동합니다.
* DirectCloud-SHIELD DLP를 계약한 경우, 사용자 페이지에 DLP 메뉴가 표시되고 사용자 휴지통에 DLP 탭이 표시됩니다.
* DirectCloud-CONNECT를 이용할 수 있는 경우, 사용자 페이지에 Connect 메뉴가 표시되고 사용자 휴지통에 Connect 탭이 표시됩니다.
* Warm Storage를 이용할 수 있는경우 사용자 페이지에 Warm Storage 메뉴가 표시되고 사용자 휴지통에 Warm Storage 탭이 표시됩니다.
* Cold Storage를 계약한 경우, 사용자 페이지에 Cold Storage 메뉴가 표시되고 사용자 휴지통에 Cold Storage 탭이 표시됩니다.
*   Cold Storage는 삭제 제한이 있기 때문에, 업로드·이동·자동 이동된 후 90일 동안 파일을 삭제할 수 없습니다. 90일이 경과하지 않은 경우, 이 매뉴얼의 절차에 따라 파일을 삭제하려고 해도 삭제 작업을 선택할 수 없습니다.

    단, Cold Storage에서도 빈 폴더는 제한 없이 삭제할 수 있습니다.습니다." 메시지에는 취소 버튼이 표시되지 않습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 폴더 삭제**
{% endhint %}

1. Shared Box를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1190).png" alt=""><figcaption></figcaption></figure>

\
**\[1 계층의 폴더 삭제]**

1. 삭제하고 싶은 폴더를 체크해, 상단의 '삭제'버튼을 클릭합니다. 여러 폴더를 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1189).png" alt=""><figcaption></figcaption></figure>



2. 확인 화면에서 텍스트 상자에 DELETE를 입력하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1191).png" alt=""><figcaption></figcaption></figure>

삭제가 시작되고 상태 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1192).png" alt=""><figcaption></figcaption></figure>



3. 삭제가 완료되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1193).png" alt=""><figcaption></figcaption></figure>



**\[2계층 이하의 폴더 삭제]**

1. 삭제할 폴더가 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1194).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나로 폴더를 삭제합니다.

❶ 삭제할 폴더에 체크를 하고 상단의 '삭제' 버튼을 클릭합니다. 여러 폴더를 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1195).png" alt=""><figcaption></figcaption></figure>

❷ 삭제하고자 하는 폴더를 체크하고, 마우스 오른쪽 버튼을 클릭하여 표시된 메뉴에서 \[삭제]를 클릭합니다. 여러 폴더를 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1196).png" alt=""><figcaption></figcaption></figure>

❸ 삭제할 폴더의 오른쪽에 있는 ▼ 버튼을 클릭하고 표시된 메뉴에서 삭제를 클릭합니다. 여러 폴더를 선택할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (1197).png" alt=""><figcaption></figcaption></figure>

삭제가 시작되고 상태 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1198).png" alt=""><figcaption></figcaption></figure>



3. 삭제가 완료되었는지 확인합니다. 취소 버튼을 클릭하면 삭제를 취소할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1199).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서  2계층 이하의 폴더 삭제**
{% endhint %}

1. 삭제할 폴더가 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1200).png" alt=""><figcaption></figcaption></figure>



2. 복사할 폴더를 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 삭제를 클릭합니다.\
   여러 폴더를 선택하여 삭제할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1201).png" alt=""><figcaption></figcaption></figure>

폴더 삭제 화면이 표시됩니다.



3. 예를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1202).png" alt=""><figcaption></figcaption></figure>



4. 폴더가 삭제되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1203).png" alt=""><figcaption></figcaption></figure>
