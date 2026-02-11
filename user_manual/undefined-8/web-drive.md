---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-8/web-drive
---

# \[Web, Drive] 파일이 자동 이동된 이력을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는, 사용자 페이지의 '자동이동 이력' 메뉴에서 Warm Storage 또는 Cold Storage로 자동 이동된 파일 목록을 표시하고, 자동 이동 이력을 확인하는 절차에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* Warm Storage를 이용할 수 있는 경우, 사용자 페이지에 「Warm Storage」 메뉴가 표시됩니다.
* Cold Storage를 계약한 경우에는 사용자 페이지에 「Cold Storage」 메뉴가 표시됩니다.
* Warm Storage 또는 Cold Storage 중 하나라도 이용할 수 있는 경우, 사용자 페이지에 「자동이동 이력」 메뉴가 표시됩니다.
* 자동 이동 이력을 확인할 수 있는 것은, 자신에게 접근 권한이 있는 이동 원본 폴더에 저장된 파일만 해당됩니다.\
  파일이 자동으로 이동된 후, 폴더에 대한 접근 권한이 사라지더라도 「자동 이동 이력」에 추가된 기록은 삭제되지 않습니다.\
  단, 이후 새로 자동 이동된 파일의 기록은 추가되지 않습니다.
* Guest에게는 「자동이동 이력」 메뉴가 표시되지 않습니다.
* 「자동이동 이력」 메뉴의 파일은 기본적으로 「자동 이동 일시」의 내림차순(최신 순)으로 표시됩니다.\
  헤더 항목의 「자동 이동 일시」를 클릭하면 내림차순(기본값)과 오름차순을 전환할 수 있습니다.\
  단, 폴더 및 파일 목록과 달리 정렬 설정은 저장되지 않으며, 웹 브라우저를 다시 시작하면 기본 상태로 돌아갑니다.
* 자동 이동 이력 상단의 헤더에서 표시 너비를 변경할 수 없습니다.
* 자동 이동 이력을 삭제할 수 없습니다.
* 「자동이동 이력」 메뉴에서는 자동 이동된 파일을 미리보기 할 수 없습니다.
* 「자동이동 이력」 메뉴에 기본적으로 표시되는 이력은 아래와 같습니다.\
  · Web 브라우저: 최근 30일 (표시 개수 제한 없음, 스크롤할 때마다 30건씩 추가로 로드됨)\
  · DirectCloud 드라이브: 최근 30일 (최대 50건)
* DirectCloud 드라이브는 Cold Storage를 지원하지 않습니다.\
  따라서, DirectCloud 드라이브의 「자동 이동 이력」 메뉴에서는 Cold Storage로 자동 이동된 이력을 확인할 수 없습니다.
* 또한 DirectCloud 드라이브에서는 파일명이나 기간으로 자동 이동 이력을 필터링하여 표시할 수 없습니다.

### 절차

{% hint style="info" %}
**Web 브라우저에서 자동이동 이력을 확인하기**
{% endhint %}

1. 사용자 페이지에서 「자동이동 이력」 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 095753.png" alt=""><figcaption></figcaption></figure>

자동 이동 이력이 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 100115.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="71.5">No.</th><th width="139.5">명칭</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>이름</td><td><p></p><p>Warm Storage 또는 Cold Storage로 자동 이동된 파일의 이름이 표시됩니다.<br>또한, 그 아래에는 현재 파일 상태에 따라 다음 중 하나의 정보가 표시됩니다.</p><ul><li>파일이 Warm Storage, Cold Storage, Shared Box, My Box 중 어느 하나에 있는 경우<br>자동 이동된 파일이 현재 저장되어 있는 폴더의 경로가 표시됩니다. 클릭하면 해당 폴더로 이동합니다.</li><li>파일이 삭제된 경우<br>사용자의 휴지통 경로가 표시됩니다. 클릭하면 휴지통으로 이동합니다.</li><li>파일이 완전히 삭제되었거나 관리자의 휴지통으로 이동한 경우<br>「삭제됨」이라고 표시됩니다.</li></ul></td></tr><tr><td>❷</td><td>원위치</td><td>자동 이동된 파일이 저장되어 있던 폴더의 경로가 표시됩니다.</td></tr><tr><td>❸</td><td>자동이동 위치</td><td>자동 이동을 통해 이동된 Warm Storage 또는 Cold Storage 폴더의 경로가 표시됩니다.</td></tr><tr><td>❹</td><td>자동이동 날짜</td><td>폴더 속성 설정에 따라 파일이 Warm Storage 또는 Cold Storage로 자동 이동된 날짜와 시간이 표시됩니다.</td></tr></tbody></table>

{% hint style="info" %}
**Web 브라우저에서 자동 이동 이력을 필터링하여 표시하기**
{% endhint %}

자동 이동 이력은 파일 이름과 기간으로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 100657.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="116">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>파일 이름에 포함된 키워드를 입력합니다.</td></tr><tr><td>❷</td><td>자동 이동 이력을 표시할 기간을 지정합니다.<br>최대 지난 12개월 이내의 기간을 지정할 수 있습니다.<br>날짜를 클릭하면 달력에서 날짜를 선택할 수 있습니다.</td></tr></tbody></table>

{% hint style="info" %}
**DirectCloud 드라이브에서 자동 이동 이력을 확인하기**
{% endhint %}

1. DirectCloud 드라이브에 로그인합니다.
2. 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브의 설정 화면이 표시됩니다.
3. ‘자동 이동 이력’을 클릭합니다.\
   자동 이동 이력이 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 101613.png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="75">No.</th><th width="152.5">명칭</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>이름</td><td><p></p><p>Warm Storage로 자동 이동된 파일의 이름이 표시됩니다.<br>또한, 그 아래에는 현재 파일의 상태에 따라 아래의 정보 중 하나가 표시됩니다.</p><ul><li>파일이 Warm Storage, Shared Box, My Box 중 어느 하나에 있는 경우<br>자동 이동된 파일이 현재 저장되어 있는 폴더의 폴더 경로가 표시됩니다. 클릭하면 해당 폴더로 이동합니다.</li><li>파일이 삭제된 경우<br>사용자의 휴지통 경로가 표시됩니다. 클릭하면 휴지통으로 이동합니다.</li><li>파일이 완전히 삭제되었거나 관리자 휴지통으로 이동된 경우<br>‘삭제됨’이라고 표시됩니다.</li></ul></td></tr><tr><td>❷</td><td>자동 이동된 날짜</td><td>폴더 속성의 설정에 따라, 파일이 Warm Storage로 자동 이동된 날짜가 현재 날짜를 기준으로<br>‘○일 전’, ‘○개월 전’의 형식으로 표시됩니다.</td></tr></tbody></table>
