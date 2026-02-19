---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/account_settings/d_letter
---

# DirectCloud 드라이브에서 폴더 경로에 할당된 드라이브 문자를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 관리 페이지에서 설정된 폴더 경로의 드라이브 문자 할당 설정을 DirectCloud Drive에서 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 2023년 6월 8일(목) 업데이트에서 드라이브 문자 설정이 드라이브 문자 할당 설정으로 변경되었습니다.\
  기존 드라이브 문자 설정에서 지정되어 있던 드라이브 문자는 드라이브 문자 할당 설정의 /DirectCloud/ 항목에 그대로 승계됩니다.
* 관리 페이지에서 폴더 경로에 드라이브 문자를 할당하는 방법의 절차에 따라 드라이브 문자가 지정된 경우, 이 매뉴얼의 절차로는 드라이브 문자를 변경할 수 없습니다.
* 사용자가 DirectCloud Drive에 로그인한 후 관리 페이지에서 폴더 경로의 드라이브 문자 설정이 변경된 경우, 사용자가 애플리케이션을 재시작하면 변경 사항이 반영됩니다.
* DirectCloud Drive에 로그인하지 않은 상태에서는 드라이브 문자 할당 설정 화면을 표시할 수 없습니다.
* 관리자가 할당한 드라이브 문자가 이미 Windows에서 사용 중인 경우, 해당 폴더는 Windows에 마운트되지 않습니다.
* 루트 폴더 /DirectCloud/에 할당된 드라이브 문자가 이미 Windows에서 사용 중인 경우, DirectCloud Drive 로그인 후 “드라이브 문자 ○가 이미 사용 중입니다.”라는 오류 메시지가 표시됩니다.
* 드라이브 문자 할당 설정에서 관리되는 폴더 경로에 포함된 폴더명이 변경되거나 폴더가 이동된 경우, 폴더 경로도 자동으로 변환됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**폴더 경로에 할당된 드라이브 문자 확인**
{% endhint %}

폴더 경로에 할당된 드라이브 문자는 "드라이브 문자 설정" 화면에서 확인할 수 있습니다.

1. DirectCloud 드라이브에 로그인합니다.<br>
2. 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (789).png" alt=""><figcaption></figcaption></figure>



3. 설정 화면의 오른쪽 상단에 있는 “⁝” 버튼을 클릭하고 표시된 고급 설정 메뉴에서 “드라이브 문자 설정”을 선택합니다.

<figure><img src="../../.gitbook/assets/image (791).png" alt=""><figcaption></figcaption></figure>

드라이브 문자 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (792).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="153">항목</th><th>설명</th></tr></thead><tbody><tr><td>드라이브 문자</td><td><p>폴더 경로에 할당된 드라이브 문자가 표시됩니다.<br><br><strong>자동 할당:</strong><br>사용자가 DirectCloud Drive에 로그인하면 드라이브 문자가 자동으로 할당됩니다.<br></p><p><strong>A~Z(C 제외):</strong> <br>25개의 문자 중 하나가 표시됩니다.<br>관리자가 설정한 고정 드라이브 문자가 표시되며, 사용자는 드라이브 문자를 변경할 수 없습니다.</p></td></tr><tr><td>마운트 상태</td><td><p>드라이브 문자가 정상적으로 할당되었는지에 대한 정보가 표시됩니다.<br>할당 설정에서 오류가 발생한 경우에는 다음과 같은 메시지가 표시됩니다.<br></p><p><strong>접근 권한 없음:</strong><br>드라이브 문자가 할당된 폴더 경로에 접근 권한이 없는 경우 표시됩니다.<br></p><p><strong>문자 사용 중:</strong><br>사용 중인 Windows 환경에서 다른 드라이브 문자가 이미 사용 중인 경우 표시됩니다.</p><p></p><p><strong>위치 없음:</strong></p><p>폴더가 삭제된 경우 표시됩니다.</p><p></p><p><strong>문자 수 초과:</strong><br>폴더 경로의 문자 수가 입력 가능한 한도를 초과한 경우 표시됩니다.</p></td></tr><tr><td>연결 위치</td><td>드라이브 문자가 할당된 폴더 경로가 표시됩니다.<br>DirectCloud Drive에서는 드라이브 문자 할당 설정을 할 수 없습니다.</td></tr></tbody></table>



{% hint style="warning" %}
**"드라이브 문자 설정" 화면의 자동 표시 설정을 전환합니다.**
{% endhint %}

DirectCloud 드라이브에 로그인할 때 드라이브 문자 할당 설정 화면을 표시할지 여부를 전환할 수 있습니다.

1. 드라이브 문자 할당 설정 화면을 자동으로 표시하도록 하려면, 드라이브 문자 할당 설정 화면에서 “로그인 또는 재시작 시 해당 창 보기'에체크합니다.\
   다시 자동 표시되지 않도록 설정하려면 체크를 해제하십시오.

<figure><img src="../../.gitbook/assets/image (793).png" alt=""><figcaption></figcaption></figure>



2. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (794).png" alt=""><figcaption></figcaption></figure>



3. DirectCloud 드라이브에서 로그아웃한 다음 다시 로그인합니다.



4. 드라이브 문자 할당 설정 화면의 자동 표시 설정이 전환되었는지 확인합니다.



{% hint style="warning" %}
**드라이브 문자를 지정하여 할당**
{% endhint %}

폴더 경로에 드라이브 문자의 자동 할당이 설정되어 있는 경우, 사용자가 드라이브 문자를 직접 지정할 수 있습니다.

1. 드라이브 문자 할당 설정 화면의 드라이브 문자 열에서, 폴더 경로에 할당할 드라이브 문자를 선택합니다.\
   이미 사용 중인 드라이브 문자는 드롭다운 메뉴에 표시되지 않습니다.

<figure><img src="../../.gitbook/assets/image (795).png" alt=""><figcaption></figcaption></figure>



2. 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (796).png" alt=""><figcaption></figcaption></figure>



3. "드라이브 문자 설정값이 정상적으로변경되었습니다."라는 화면이 나타납니다.\
   확인 버튼을 클릭합니다.\
   드라이브가 재시작 됩니다.

<figure><img src="../../.gitbook/assets/image (797).png" alt=""><figcaption></figcaption></figure>



4. Windows 탐색기에서 지정한 드라이브 문자로 변경되었는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (798).png" alt=""><figcaption></figcaption></figure>
