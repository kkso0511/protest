---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/access_permission/delete_permission
---

# 사용자 페이지에서 사용자의 접근 권한을 삭제하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 <전체권한> 접근 권한이 부여된 사용자가 사용자 페이지에서 다른 사용자의 접근 권한을 삭제하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 Shared Box와 Connect 폴더에서의 작업 방법을 설명하고 있지만, 다른 폴더에서도 동일한 절차로 설정할 수 있습니다.
* ‘접근 권한’이란 폴더나 파일을 조작할 수 있는 권한을 의미합니다.
* ‘접근 권한 레벨’은, 접근 권한이 부여된 폴더 내의 폴더나 파일에 대해 어떤 작업이 가능한지를 정의한 것입니다.\
  접근 권한의 상세 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission)을 참조해주시기 바랍니다.
* 이 매뉴의 절차를 실행하려면 다음과 같이 설정되어 있어야 합니다.
  * 관리자 페이지의 '공유설정'->'Shared Box 관리' 에서 이용할 폴더를 클릭하면 나타나는 우측의 설정항목에서 '권한 관리 확대’를 ‘사용’으로 설정
  * 사용자에게 <전체권한> 접근 권한 부여
* Connect 폴더, Warm Storage, Cold Storage에서는 Guest 초대를 사용할 수 없으므로 Guest 설정은 불가능합니다.
* <마스터> 권한이 부여된 사용자는 접근 권한 확장이 설정되지 않은 경우에도 본 문서의 절차로 접근 권한을 부여할 수 있습니다.
* 접근 권한 및 접근 권한 레벨은 최대 6계층까지 설정할 수 있습니다.
* 접근 권한 설정 확장은 제1계층 폴더에 대해 설정하며, 설정 내용은 하위 폴더에 상속됩니다.
* 다음 화면에서는 각각 최대 3,000건까지 접근 권한을 설정할 수 있으며, 3,000건을 초과하면 ‘확인’ 버튼이 비활성화됩니다.
  * 사용자 접근 권한 설정 화면
  * Guest 접근 권한 설정 화면
* 사용자가 설정한 접근 권한은 ‘로그 현황’ > ‘전체권한자 권한변경 내역’ 메뉴에서 확인할 수 있습니다.
* 해당 메뉴에서는 ‘누가 어떤 폴더의 권한을 변경했는가’를 확인할 수 있지만, ‘누구에게 어떤 권한을 부여했는가’는 확인할 수 없습니다.
* 폴더 접근 권한을 가진 사용자의 정보를 사용자 페이지에 표시하는 방식에 따라, ‘관리자 설정에 의해 일부 공유자 정보만 제공될 수 있습니다.’라는 메시지가 나타날 수 있습니다.\
  이 경우, 사용자가 직접 초대한 Guest라 하더라도 접근 권한 레벨을 변경할 수 없는 경우가 있습니다.
* 옵션 ‘DirectCloud-SHIELD DLP’를 이용 중인 경우 ‘DLP’ 메뉴가 표시됩니다.
* Warm Storage를 사용할 수 있는 경우, ‘Warm Storage’ 메뉴가 표시됩니다.
* Cold Storage를 계약한 경우 ‘Cold Storage’ 메뉴가 표시됩니다.
* Cold Storage에서는 제1계층 폴더에 대해서만 접근 권한을 설정할 수 있으며, 설정 내용은 하위 폴더에 상속됩니다.
* Cold Storage에서는 다운로드 및 미리보기를 사용할 수 없기 때문에 ‘다운로더’ 또는 ‘프리뷰어’ 권한을 부여할 수 없습니다.
* Cold Storage 폴더에서 설정할 수 있는 접근 권한은 최대 100건까지이며, <마스터>는 제외됩니다.
* Cold Storage에서는 접근 권한 설정 시 ‘그룹’을 선택할 수 없습니다.
* 폴더를 Cold Storage로 이동하면 해당 폴더의 접근 권한 정보는 삭제됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**사용자 또는 Guest 접근 권한 삭제**
{% endhint %}

**\[접근 권한을 삭제할 폴더 선택]**

1. 접근 권한을 삭제할 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1187).png" alt=""><figcaption></figcaption></figure>



**\[그룹 사용자의 접근 권한 삭제]**

1. 슬라이드 화면의 '폴더 속성' 설정에서 '사용자/그룹'의 '권한관리' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1188).png" alt=""><figcaption></figcaption></figure>

&#x20;      사용자 접근 권한 설정 화면이 표시됩니다.



2. 접근 권한을 삭제할 그룹 또는 사용자의 '×' 버튼을 클릭합니다.

![](<../../.gitbook/assets/스크린샷 2025-11-03 143543.png>)

&#x20;      오른쪽 영역에서 그룹 또는 사용자가 삭제됩니다.



3. 확인 버튼을 클릭합니다.

![](<../../.gitbook/assets/스크린샷 2025-11-03 143543 (1).png>)

&#x20;      권한 설정이 저장됩니다.



4. 공유중인 사용자의 사용자/그룹 아이콘에서 삭제된 그룹 사용자만큼 수가 줄어들었는지 확인합니다.

![](<../../.gitbook/assets/스크린샷 2025-11-03 143707.png>)



**\[Guest 접근 권한 삭제]**

1. 슬라이드 화면의 '폴더 속성' 설정에서 'Guest'의 '권한관리' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1023).png" alt=""><figcaption></figcaption></figure>

&#x20;     Guest 접근 권한 설정 화면이 표시됩니다.



2. 접근 권한을 삭제할 Guest의 오른쪽에 있는 '×' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1024).png" alt=""><figcaption></figcaption></figure>

&#x20;     오른쪽 영역에서 Guest가 삭제됩니다.



3. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1026).png" alt=""><figcaption></figcaption></figure>

&#x20;      접근 권한 설정이 저장됩니다.



4. 공유중인 사용자의 Guest 아이콘에서 삭제한 Guest 만큼 숫자가 줄어들었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1027).png" alt=""><figcaption></figcaption></figure>
