---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/undefined-3
---

# 업로드한 파일을 판정 기준에 따라 보안하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약한 경우, IRM(Information Rights Management)을 이용하여 의도하지 않은 파일 반출로 인한 정보 유출을 방지할 수 있습니다.\
이 매뉴얼 에서는 [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 생성한 문서 속성에 따라 다음 처리가 이루어지도록 설정하는 방법을 설명합니다.

* 보안등급에 따른 라벨 추가
* irm 확장자 추가
* 파일 암호화(스토리지 외부로 반출되었을 때)
* '사외비', 'Confidential' 등의 워터마크(투명 문자) 추가

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* DirectCloud-SHIELD IRM을 사용할 수 있는 상태라 하더라도, [특정 폴더에서 DirectCloud-SHIELD IRM을 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-4/directcloud-shield-irm)에서 사용 여부를 사용하지 않음으로 설정한 경우에는 암호화가 적용되지 않습니다.

### 절차

{% hint style="info" %}
**'보안수준 정의' 화면을 표시합니다.**
{% endhint %}

1. 'SHIELD' > '설정' 메뉴를 선택하고 '보안수준 정의' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (258).png" alt=""><figcaption></figcaption></figure>

2. 동작 열에 표시된 버튼을 클릭합니다.\
   업로드 대상 파일이, [보안 문서 판단 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 지정한 문서 속성 중 어느 항목에 해당하는지 확인한 뒤, 그에 맞는 보안수준을 선택합니다.

<figure><img src="../../.gitbook/assets/image (259).png" alt=""><figcaption></figcaption></figure>

&#x20;      선택한 보안수준의 보안수준 정의 화면이 표시됩니다.

{% hint style="info" %}
**스토리지 외부로 반출된 파일이 암호화되도록 설정합니다.**
{% endhint %}

**보안수준 정의에서 저장 방식 설정하기**

1.  '보안수준 정의'  > '반입 문서보안' > '라벨 표시 후 암호화 저장' 선택하고 '저장' 버튼을 클릭합니다.<br>

    **NOTE**\
    라벨 표시 후 암호화를 선택하면, 스토리지 외부로 파일이 반출될 때 해당 파일이 암호화되도록 설정됩니다.

<figure><img src="../../.gitbook/assets/image (260).png" alt="" width="563"><figcaption></figcaption></figure>

이 설정에 따라 IRM의 문서 속성에 맞게 업로드된 파일에 보안등급 라벨이 표시됩니다.\
암호화 없이 보안등급 라벨만 표시하려면 '라벨만 표시'를 선택해 주세요.



**저장 방식 설정에 따른 표시 차이**

파일을 업로드하면 저장 방식 설정에 따라 아래와 같이 표시됩니다.

* 저장 방식에서 라벨 표시 후 암호화를 선택한 경우\
  파일을 업로드하면 보안등급 라벨이 표시되고, 파일의 확장자가 .irm으로 변경됩니다.

<figure><img src="../../.gitbook/assets/image (261).png" alt=""><figcaption></figcaption></figure>

* 저장 방식에서 라벨만 표시를 선택한 경우\
  파일을 업로드하면 보안등급 라벨이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (264).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**업로드한 파일에 워터마크를 표시합니다.**
{% endhint %}

**보안수준 정의에서 워터마크 설정하기**

1. '보안수준 정의' > '반입 문서 보안' > '워터마크' 에서 '사용'을 선택하고, 상세설정▼를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (266).png" alt="" width="563"><figcaption></figcaption></figure>

&#x20;      워터마크 화면이 표시됩니다.

2. 워터마크를 설정한 뒤 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (267).png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="182.79998779296875">항목</th><th>설명</th></tr></thead><tbody><tr><td>표시정보</td><td><p>워터마크에 표시할 정보에 체크합니다.<br>표시할 수 있는 정보는 다음과 같습니다.</p><ul><li><strong>사용자 ID</strong><br>파일을 미리보기 한 사용자의 ID</li><li><strong>시간</strong><br>파일을 미리보기 한 날짜와 시간</li><li><strong>보안등급</strong><br>보안수준 정의에 표시되어 있는 보안등급</li><li><strong>추가 정보</strong><br>추가정보에 체크한 경우, 표시할 문자열을 100자 이내로 입력합니다.</li></ul></td></tr><tr><td>글자색상</td><td>▼ 버튼을 클릭하여 워터마크 텍스트의 색상을 선택합니다.</td></tr><tr><td>글자크기</td><td>슬라이드 버튼을 움직여 워터마크 텍스트의 크기를 설정합니다.<br>텍스트를 굵게 표시하려면 굵게에 체크합니다.</td></tr><tr><td>투명도</td><td>슬라이드 버튼을 움직여 워터마크의 투명도를 설정합니다.<br>투명도를 100%로 설정하면 워터마크가 표시되지 않게 됩니다.</td></tr><tr><td>표시 위치</td><td>워터마크의 표시 위치 정보가 표시됩니다.<br>표시 위치를 변경하려면 타일 버튼에서 변경할 영역을 선택합니다.</td></tr></tbody></table>



**워터마크 표시 예**

아래에 워터마크 설정 예시와 표시 예시를 제공합니다.

* 워터마크 설정 예시

<figure><img src="../../.gitbook/assets/image (268).png" alt="" width="563"><figcaption></figcaption></figure>

* 사용자 페이지에서 파일을 미리보기 한 경우의 예

<figure><img src="../../.gitbook/assets/image (269).png" alt=""><figcaption></figcaption></figure>
