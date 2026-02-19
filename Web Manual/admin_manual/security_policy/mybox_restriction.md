---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/security_policy/mybox_restriction
---

# 특정 그룹이나 사용자에게 My Box 사용을 허용하지 않도록 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '보안 정책' > '사용 권한' 메뉴에서 그룹이나 사용자에게 적용된 My Box 기능을 제외하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 표준 상태에서는 그룹·사용자에게 모든 기능(My Box, 링크, 첨부파일 전송, 업로드 요청, Shared Box)이 적용됩니다.
* 사용자가 여러 그룹에 소속되어 있는 경우, 사용 권한 설정은 해당 사용자에게 합산되어 적용됩니다.\
  예를 들어 아래와 같이 설정되어 있는 경우, 사용자에게는 모든 권한이 적용됩니다.
  * **예:**\
    A부(My Box만), B부(링크만), C부(첨부파일 전송만), D부(업로드 요청만), E부(Shared Box만)에 소속되어 있는 경우
* 최상위에 있는 회사명 그룹에는 기본적으로 모든 기능 사용(기본값) 설정이 적용되어 있습니다.\
  하위 그룹에 소속된 사용자에게는 최상위 그룹의 기능 제한 설정이 합산되어 적용되므로, 특정 그룹에 특정 기능만 사용하도록 하고 싶은 경우에는 회사명 그룹에 모든 기능을 사용하지 않도록 설정을 먼저 적용한 후, 그룹별로 사용 권한 설정을 등록해야 합니다.
* 사용 권한 설정 메뉴의 설정은 Guest에게는 적용되지 않습니다.
* 사용 권한 설정은 최대 30건까지 등록할 수 있습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**사용 권한 설정 추가**
{% endhint %}

1. '보안 정책' > '사용 권한' 메뉴를 선택하고 권한 추가 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (632).png" alt=""><figcaption></figcaption></figure>



2. 권한 이름을 입력하고 적용할 기능을 선택합니다. 'My Box' 항목을 선택 취소한 상태에서 '저장' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (639).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**그룹에 적용된 My Box 기능 제외**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 선택하고 My Box 기능을 제외할 그룹을 선택한 다음 수정 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (634).png" alt=""><figcaption></figcaption></figure>



2. 사용 권한에서 만든 권한 이름을 선택하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (640).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자에게 적용된 My Box 기능 제외**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 선택하고 My Box 기능을 제외할 사용자를 선택하고 편집 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (636).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하여 사용 권한의 자세히 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (637).png" alt=""><figcaption></figcaption></figure>



3. 해당 사용자의 사용 권한을 '소속 그룹에 상관없이 단일 권한 강제 적용'을 선택하고 사용 권한에서 만든권한을 선택한 다음 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (641).png" alt=""><figcaption></figcaption></figure>
