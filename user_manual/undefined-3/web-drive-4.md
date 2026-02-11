---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-3/web-drive-4
---

# \[Web, Drive] 파일을 복사하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 Web 브라우저 또는 DirectCloud 드라이브를 사용하여 DirectCloud에 저장된 파일을 DirectCloud의 다른 폴더로 복사하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 Shared Box에서의 조작 방법을 기준으로 설명하고 있지만, Shared Box 외의 위치에서도 동일한 절차로 이용하실 수 있습니다.
*   파일 복사 기능은 내부적으로 먼저 원본 파일을 복사한 뒤, 대상 폴더로 업로드하는 방식으로 처리됩니다.\
    따라서 파일을 복사하는 사용자에게는 원본 폴더와 대상 폴더 모두에서 아래의 접근 권한이 필요합니다.

    * 원본 폴더:\
      <마스터>, <전체권한>, <편집자>
    * 대상 폴더:\
      <마스터>, <전체권한>, <편집자>, <편집자－>, <프리뷰어＋>, <업로더>

    자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/web), [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/directcloud)을 참고해 주시기 바랍니다.
* 복사 화면에서 대상 폴더에 새 폴더를 생성하려면 '마스터', '전체권한' 접근 권한이 필요합니다.
* 다음의 모든 조건에 해당하는 경우, DirectCloud 드라이브에서 파일을 이동할 수 없습니다.
  * [워크플로우를 사용하는 방법](https://help.directcloud.net/admin_manual/undefined-7/undefined)에서 워크플로우가 활성 상태로 설정되어 있음
  * [특정 폴더에서 워크플로우를 사용하도록 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-20)에서 원본 폴더 또는 대상 폴더의 워크플로우가 사용함으로 설정되어 있음
  * 다운로드 워크플로우 또는 업로드 워크플로우의 신청자로 설정되어 있음
* Warm Storage 및 Cold Storage에서는 폴더와 파일을 복사하는 기능을 제공하지 않습니다.\
  따라서 아래 방향으로 폴더 및 파일 복사가 불가능합니다.
  * Hot Storage     ➡️ Warm Storage\
    　　          　    ➡️ Cold Storage
  * Warm Storage ➡️ Hot Storage\
    　　　　           ➡️ Cold Storage
  * Warm Storage ➡️ Warm Storage\
    Cold Storage    ➡️ Cold Storage
* 여러 개의 폴더와 파일을 선택한 경우, 선택된 목록의 위에서부터 순서대로 복사가 실행됩니다.
* 대상 폴더에 동일한 이름의 파일이 존재하는 경우에는 복사할 수 없습니다.
* 이미 링크가 생성된 파일을 복사하는 경우, 링크 정보는 복사되지 않습니다.\
  반면, 파일을 이동하는 경우에는 링크 정보가 유지됩니다.
* 한 번에 복사할 수 있는 파일 수에는 제한이 없습니다.\
  다만, 처리 부하로 인해 속도가 저하될 수 있으므로 DirectCloud에서는 한 번에 1,000개 이상의 폴더 및 파일을 복사하는 작업은 권장하지 않습니다.
* 여러 폴더와 파일을 동시에 복사할 때, 한 번에 복사할 수 있는 하위 폴더의 총수는 10,000개입니다.\
  10,001개 이상의 하위 폴더를 포함한 상위 폴더를 복사하려고 하면\
  "복사 또는 이동 대상이 최대값(10,000개)을 초과하여 조작을 진행할 수 없습니다."\
  라는 오류 메시지가 표시되며, 복사 처리는 중단됩니다.
*   복사 작업 중 상태 화면의 "×"를 클릭하거나, 세션 시간 10분을 초과한 경우에는\
    "복사/이동 중 타임아웃이 발생하여 더 이상 진행할 수 없습니다."\
    라는 오류 메시지가 표시됩니다.

    이 경우 오류 메시지가 표시되기 전까지 이미 처리된 폴더 및 대상 폴더에 저장된 폴더·파일은 복사되지만, 처리 대기 중이던 폴더·파일은 복사되지 않습니다.
* DirectCloud AI가 활성화된 폴더에서의 파일 복사 가능 범위는 다음과 같습니다.
  * DirectCloud AI가 활성화된 폴더로 파일을 복사할 수 있는 폴더:\
    My Box, Shared Box, 문서 관리 폴더
  * DirectCloud AI가 활성화된 폴더에서 파일을 복사할 수 있는 폴더:\
    My Box, Shared Box, 문서 관리 폴더, Connect 폴더, DLP 폴더
*   DirectCloud AI가 활성화된 폴더로 파일을 복사하거나 이동하는 경우, 벡터 데이터가 생성됩니다.\
    벡터 데이터 생성 시에는 파일에 포함된 텍스트의 용량 등에 따라 비용이 발생하므로 주의가 필요합니다.

    DirectCloud AI에서 생성되는 벡터 데이터에 대한 상세 내용은 [DirectCloud AI 사양 및 참고 사항](https://help.directcloud.net/admin_manual/directcloud-ai/directcloud-ai-4)을 참고해 주십시오.
* DirectCloud AI가 활성화된 폴더에서는 벡터 데이터 생성 중인 파일을 복사할 수 없습니다.
* Windows 탐색기 기능으로 DirectCloud-SHIELD IRM에서 irm 확장자가 추가된 파일을 포함한 여러 파일을 선택해 복사하는 경우, IRM으로 암호화된 파일은 복사에 실패하지만 암호화되지 않은 파일은 정상적으로 복사됩니다.

***

### 절차

{% hint style="warning" %}
**Web 브라우저에서 파일 복사하기**
{% endhint %}

1. 복사하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2423).png" alt=""><figcaption></figcaption></figure>



2. 다음 중 하나의 방법으로 파일의 복사 화면을 표시합니다.

➊ 복사하려는 파일에 체크한 뒤, 상단의 복사 버튼을 클릭합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2424).png" alt=""><figcaption></figcaption></figure>

➋ 복사하려는 파일에 체크한 후, 마우스 오른쪽 버튼을 클릭하여 표시된 메뉴에서 복사를 선택합니다. 여러 파일을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2425).png" alt=""><figcaption></figcaption></figure>

➌ 복사하려는 파일의 오른쪽에 있는 ▼ 버튼을 클릭한 뒤, 표시된 메뉴에서 복사를 선택합니다. 이 방법에서는 여러 파일을 선택할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (2426).png" alt=""><figcaption></figcaption></figure>

➍ 복사 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2427).png" alt="" width="563"><figcaption></figcaption></figure>



3. 복사 대상 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2428).png" alt="" width="563"><figcaption></figcaption></figure>



4. 필요에 따라 새 폴더를 클릭하여 새 폴더를 생성합니다.

<figure><img src="../../.gitbook/assets/image (2429).png" alt="" width="563"><figcaption></figcaption></figure>



5. 복사 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2430).png" alt="" width="563"><figcaption></figcaption></figure>

복사가 시작되며 상태 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-12-04 092932.png" alt="" width="563"><figcaption></figcaption></figure>



6. 복사가 완료되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2431).png" alt="" width="563"><figcaption></figcaption></figure>

실행행취소 버튼을 클릭하면 복사 작업을 취소할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2432).png" alt="" width="563"><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 파일 복사하기**
{% endhint %}

**\[Windows 탐색기 기능으로 복사하기]**

1. 복사하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2433).png" alt=""><figcaption></figcaption></figure>



2. 복사하려는 파일을 마우스 오른쪽 버튼으로 클릭하고, 표시된 메뉴에서 복사를 선택합니다.\
   여러 파일을 선택하여 복사할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (2434).png" alt=""><figcaption></figcaption></figure>



3. 복사 대상 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2435).png" alt=""><figcaption></figcaption></figure>



4. 파일을 선택하지 않은 상태에서 마우스 오른쪽 버튼을 클릭하고, 표시된 메뉴에서 붙여넣기를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2436).png" alt=""><figcaption></figcaption></figure>



5. 파일이 복사된 것을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2437).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브 기능을 사용하여 복사하기**
{% endhint %}

DirectCloud 드라이브에서 DirectCloud-SHIELD IRM의 보안등급 라벨과 irm 확장자가 추가된 파일을 복사하는 경우에는, 아래 절차에 따라 DirectCloud 드라이브 기능을 사용해 파일을 복사해야 합니다.

1. 복사하려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2438).png" alt=""><figcaption></figcaption></figure>



2. 복사하려는 파일을 마우스 오른쪽 버튼으로 클릭한 뒤, 표시된 메뉴에서 'DirectCloud-Drive' ＞ '복사'를 선택합니다.\
   여러 파일을 선택하여 복사할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (2439).png" alt=""><figcaption></figcaption></figure>



3. 저장할 폴더를 선택한 뒤 복사 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2440).png" alt=""><figcaption></figcaption></figure>



4. 파일이 복사된 것을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2441).png" alt=""><figcaption></figcaption></figure>
