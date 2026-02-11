---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-11/directcloud-1
---

# DirectCloud 드라이브에서 파일 오프라인 작업을 수행하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud 드라이브에는 오프라인 폴더에 파일을 저장하여 네트워크 연결 없이도 파일을 편집할 수 있는 오프라인 기능이 있습니다. 오프라인 폴더에서 편집한 파일은 네트워크 연결이 온라인 상태가 될 때 DirectCloud에 반영될 수 있습니다.\
이 매뉴얼에서는 DirectCloud 드라이브에서 오프라인 작업을 수행하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 오프라인 기능을 사용하려면 관리자 페이지에서 DirectCloud 드라이브의 오프라인 사용을 사용하거나 사용하지 않도록 설정하는 방법에 따라 오프라인 기능을 사용하도록 설정해야 합니다.
* 오프라인 상태에서 DirectCloud를 종료하거나 Windows를 다시 시작하면 오프라인으로 로그인한 상태가 유지됩니다.
* 폴더를 '오프라인' 폴더에 저장할 수 없습니다.
* 오프라인 폴더에서 파일을 업로드할 때 별칭으로 저장을 선택하면 파일 이름 끝에 숫자가 추가됩니다.
* 오프라인 폴더에 파일을 저장할 때 로컬 디스크 공간이 부족하면 오류가 발생합니다.
* '오프라인' 폴더에서 파일을 업로드할 때 저장용량 또는 폴더 속성의 '용량 제한'을 초과하면 오류가 발생합니다.
* 오프라인 폴더에 저장할 수 있는 파일 수의 상한은 5,000입니다.
* PC에서 오프라인 폴더에 저장된 파일을 DirectCloud에 업로드할 수 없으므로 파일을 마우스 오른쪽 버튼으로 클릭하고 DirectCloud 드라이브를 선택해도 파일 업로드 및 원래 위치 정보를 선택합니다. 할 수 없습니다.
* 오프라인 기능은 다음 응용 프로그램에서 사용할 수 있습니다.
  * Windows용 DirectCloud 드라이브
* 오프라인 폴더에 파일을 저장하려면 '다운로드' 접근 권한이 필요합니다.
* 오프라인으로 DirectCloud 드라이브에 로그인하거나 로그아웃한 기록은 DirectCloud 로그에 저장되지 않습니다.
* 오프라인으로 로그인하더라도 마지막으로 로그인했을 때 드라이브 문자 할당 정보가 드라이브를 마운트합니다.
* 오프라인 폴더에서 편집할 때 여러 사용자가 편집할 수 있는 파일을 덮어쓰려면 다음 사항에 유의해야 합니다.
  * 사용자 A가 '오프라인' 폴더에 저장한 파일을 편집할 때 사용자 B가 Shared Box의 동일한 파일을 직접 편집하여 저장하면 일단 사용자 B의 편집 내용으로 파일이 저장됩니다. 그러나 사용자 A가 편집한 파일이 '오프라인' 폴더에서 반환되면 파일을 덮어씁니다.
  * 사용자 B가 Shared Box 폴더의 파일을 편집할 때 사용자 A가 '오프라인' 폴더에 저장한 동일한 파일을 편집하여 Shared Box 폴더로 되돌리면 일단 사용자 A의 편집 내용으로 파일이 저장됩니다. 그러나 사용자 B가 편집한 파일이 저장되면 사용자 A가 리턴한 파일을 겹쳐씁니다.
* 다운로드 워크플로우가 설정된 경우 오프라인 기능을 사용할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**온라인/오프라인 상태로 이동**
{% endhint %}

**\[DirectCloud 드라이브를 오프라인 상태로 변경]**

1. 로그인 상태 유지를 선택하여 DirectCloud 드라이브에 로그인합니다.

<figure><img src="../../.gitbook/assets/image (1580).png" alt=""><figcaption></figcaption></figure>



2. 인터넷 연결을 끊습니다.



3. DirectCloud 드라이브의 고급 설정 메뉴에서 '종료'를 선택합니다.\
   세션을 유지하면서 DirectCloud 드라이브가 종료됩니다.

{% hint style="info" %}
**NOTE:**\
**'**&#xB85C;그아웃'을 선택하면 로그인 세션이 종료되므로 오프라인 기능을 사용할 수 없게 됩니다.\
반드시 '종료'를 선택하십시오.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (1581).png" alt=""><figcaption></figcaption></figure>



4. DirectCloud 드라이브를 시작합니다.\
   자동으로 오프라인 모드로 전환합니다.



**\[오프라인 상태 확인]**

1. PC의 트레이아이콘에 있는 DirectCloud 드라이브 아이콘을 보고 오프라인 상태인지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2572).png" alt=""><figcaption></figcaption></figure>



2. PC의 트레이아이콘에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   오프라인 상태 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2572).png" alt=""><figcaption></figcaption></figure>



<figure><img src="../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="157">항목</th><th>내용</th></tr></thead><tbody><tr><td>로그아웃</td><td>클릭하면 세션이 종료되고 오프라인에서 사용할 수 없습니다.<br>인터넷에 연결되어 있지 않은 상태에서 로그인 화면에서 로그인을 시도하면 "서버에 연결할 수 없습니다."라는 메시지가 표시됩니다.</td></tr><tr><td>프로그램종료</td><td>현재 세션을 유지하면서 DirectCloud 드라이브를 종료합니다. DirectCloud 드라이브를 다시 시작하면 오프라인 모드에서 DirectCloud 드라이브를 사용할 수 있습니다.</td></tr></tbody></table>



**\[DirectCloud 드라이브를 온라인 상태로 되돌리기]**

인터넷이 연결되면 자동으로 DirectCloud 드라이브가 온라인 상태로 변경됩니다.\
인터넷에 연결이 됐음에도 DirectCloud 드라이브가 오프라인 상태로 남아있다면 아래 절차대로 진행합니다.

1. PC의 트레이아이콘에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   오프라인 상태 정보가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2572).png" alt=""><figcaption></figcaption></figure>



2. 로그아웃 또는 프로그램종료를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (758).png" alt=""><figcaption></figcaption></figure>



3. DirectCloud 드라이브 로그인 화면에서 DirectCloud에 다시 로그인합니다.



{% hint style="warning" %}
**오프라인 폴더에 파일 저장**
{% endhint %}

이 매뉴얼에서는 My Box 또는 Shared Box 폴더의 파일을 '오프라인 폴더'에 저장하는 방법에 대해 설명합니다.

1. DirectCloud 드라이브에서 My Box 또는 Shared Box에 저장된 파일을 봅니다.

<figure><img src="../../.gitbook/assets/image (759).png" alt=""><figcaption></figcaption></figure>



2. 오프라인으로 편집할 파일을 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 오프라인 시 사용을을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (760).png" alt=""><figcaption></figcaption></figure>

파일이 오프라인 폴더에 복사됩니다.



{% hint style="warning" %}
**오프라인 폴더에서 파일 확인/편집**
{% endhint %}

이 매뉴얼에서는 네트워크가 오프라인 상태이고 Windows 탐색기에서 오프라인 폴더를 표시하고 저장된 파일의 정보를 확인하는 방법에 대해 설명합니다.

1. Windows 탐색기에서 DirectCloud 드라이브를 보고 오프라인 폴더를 클릭합니다.\
   오프라인인 경우 DirectCloud 드라이브 바로 아래에 오프라인 폴더만 표시됩니다.



2. 오프라인 폴더에 오프라인 저장된 파일이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (761).png" alt=""><figcaption></figcaption></figure>



3. 오프라인 폴더에서 파일을 직접 보고 편집할 수 있습니다.\
   오프라인 폴더에서는 일반 폴더와 마찬가지로 다음 작업이 가능합니다.

* 파일 표시
* 파일 이름 변경
* 파일 삭제
* 드래그 앤 드롭으로 파일 조작



4. 오프라인 폴더의 파일이 DirectCloud의 어디에 저장되는지 확인하려면 파일을 마우스 오른쪽 단추로 클릭하고 'DirectCloud-Drive' > '원위치 정보'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (762).png" alt=""><figcaption></figcaption></figure>

화면의 오른쪽 하단에 DirectCloud의 폴더 경로가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (763).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**오프라인 폴더의 파일 업로드**
{% endhint %}

이 매뉴얼에서는 네트워크에 연결할 수 있는 상태가 되면 오프라인 폴더에서 편집한 파일을 DirectCloud의 원래 폴더에 업로드하는 방법에 대해 설명합니다.

1. Windows 탐색기에서 DirectCloud 드라이브를 보고 오프라인 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (764).png" alt=""><figcaption></figcaption></figure>



2. 오프라인으로 편집한 파일을 마우스 오른쪽 단추로 클릭하고 'DirectCloud-Drive' > '업로드'를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (765).png" alt=""><figcaption></figcaption></figure>

파일이 업로드됩니다.\
네트워크에 연결할 수 없는 상태인 경우 화면 오른쪽 하단에 "서버에 연결할 수 없습니다."라는 메시지가 표시됩니다.
