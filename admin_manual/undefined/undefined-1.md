---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined/undefined-1
---

# 같은 이름의 파일 업로드 시 처리 기준 설정 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 My Box·Shared Box에 같은 이름의 파일을 업로드했을 때 어떻게 처리할지 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '보안 정책'에 접근 가능합니다.
* 업로드 대상 폴더에 업로드한 폴더와 동일한 이름의 폴더가 있고, 해당 폴더에 같은 이름의 파일이 저장되어 있는 경우에도 본 설정에 따라 저장됩니다.
* ‘업로드 시 처리’ 설정은 Web 브라우저에만 적용됩니다.
* DirectCloud 드라이브에 업로드하는 경우에는, 본 매뉴얼에서는의 절차와 관계없이 운영체제에 따른 확인 메시지가 표시됩니다.
* 공유 링크 또는 업로드 요청에 파일을 업로드하는 경우에는, 본 매뉴얼에서는의 절차와 관계없이 파일명 끝에 숫자가 추가됩니다.
* 파일이 덮어쓰기 저장되면 버전이 업데이트됩니다.
* My Box·Shared Box에 업로드 가능한 확장자를 제한하는 설정이 되어 있는 경우에는, 해당 설정이 우선 적용됩니다.
* 업로드 대상이 아래에 해당하는 경우에는, 같은 이름의 파일이 저장되어 있더라도 본 매뉴얼에서는의 절차와 관계없이 파일명 끝에 ‘-복사’가 추가되어 별도의 파일로 업로드됩니다.
  * Warm Storage
  * DirectCloud AI가 활성화된 폴더
* 아래 방법으로 파일을 업로드한 경우에는, 자동으로 파일명 끝에 숫자가 추가됩니다.
  * 공유 링크의 업로드 기능을 사용하여 파일을 업로드한 경우
  * 업로드 요청에 파일을 업로드한 경우
  * 업로드 전용 메일을 통해 파일을 업로드한 경우
  * Cold Storage에 파일을 업로드한 경우
* Cold Storage를 계약한 경우에는 관리 페이지에 Cold Storage 관리 메뉴가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**업로드 기능 관련 설정 보기**
{% endhint %}

1. '보안 정책' > '반입 정책' 메뉴를 선택합니다.

<figure><img src="../../.gitbook/assets/image (1626).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**파일이 덮어씌워 지도록 설정하기**
{% endhint %}

1. '동일 파일명 업로드'에서 덮어쓰기를 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1627).png" alt=""><figcaption></figcaption></figure>

**\[파일을 업로드할 때의 동작]**

사용자가 파일을 업로드하면 덮어쓰기되어 다음과 유사한 메시지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1628).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**업로드가 차단되도록 설정**
{% endhint %}

1. '동일 파일명 업로드'에서 '차단하기'를 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1629).png" alt=""><figcaption></figcaption></figure>

**\[파일을 업로드할 때의 동작]**

사용자가 파일을 업로드하면 다음과 유사한 오류 메시지가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1630).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**사용자가 파일을 처리하는 방법을 선택할 수 있도록 설정**
{% endhint %}

1. '동일 파일명 업로드'에서 '사용자 선택'을 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1631).png" alt=""><figcaption></figcaption></figure>

**\[파일을 업로드할 때의 동작]**

사용자가 파일을 업로드하면 '파일중복 처리' 화면이 표시됩니다.\
덮어쓰기, 건너뛰기, 다른 이름으로 업로드 중 하나를 선택하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1632).png" alt=""><figcaption></figcaption></figure>

| 항목          | 내용                                |
| ----------- | --------------------------------- |
| 파일덮어쓰기      | 이미 폴더에 저장된 같은 이름의 파일을 덮어쓰고 저장합니다. |
| 파일건너뛰기      | 업로드를 취소합니다.                       |
| 다른 이름으로 업로드 | 파일 이름 끝에 '-복사'를 추가하여 업로드합니다.      |
