---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/undefined
---

# 보안문서 판정 기준 설정 방법

### 개요

DirectCloud의 옵션인 DirectCloud-SHIELD IRM을 계약한 경우, IRM(Information Rights Management)을 이용하여 의도하지 않은 파일 반출로 인한 정보 유출을 방지할 수 있습니다.\
\
DirectCloud-SHIELD IRM에서는 아래와 같은 설정을 하실 수 있습니다.

* 업로드된 파일에 대해 보안문서의 판정 기준에 따른 라벨을 부여하는 설정&#x20;
* <사외비>, \<Confidential> 등의 워터마크(투명 문자)를 추가하는 설정
* 저장공간 외부로 반출되는 파일을 암호화하는 설정
* 반출된 파일의 보안 설정(허용하지 않는 작업, 이용 가능한 사용자, 유효 기간, 열람 가능 횟수 등)

이 매뉴얼 에서는 DirectCloud-SHIELD IRM에서 보안 문서의 판정 기준을 설정하는 방법에 대해 설명드립니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* 문서의 보안도를 판정하는 기준이 되는 특정 단어에는, 단어 간 공백을 포함하여 최대 255자까지 입력하실 수 있습니다.
* 문서의 보안등급을 판정하는 기준이 되는 특정 단어에서 파일명에 체크가 되어 있는 경우, 지정한 단어 중 하나라도 해당되면 보안 문서로 판정되므로 검출 횟수 설정은 표시되지 않습니다.
* 문서의 보안등급을 판정하는 기준이 되는 특정 단어에서는 문서 내 텍스트 또는 파일명 중 어느 한쪽의 조건을 충족하면 보안 문서 판정 대상이 됩니다.
* 여러 검출 대상을 판정 기준으로 선택하고 AND/OR 조건을 설정하는 경우, 연산자 우선순위가 아니라 왼쪽부터 순차적으로 처리됩니다.
  * 예: 개인 정보 OR 특정 단어 AND 확장자를 처리하는 경우\
    1번째 처리: 개인 정보 OR 특정 단어\
    2번째 처리: 1번째 처리 결과 AND 확장자
* 본 문서의 절차에 따라 DirectCloud-SHIELD IRM을 활성화한 경우라도, [특정 폴더에서 DirectCloud-SHIELD IRM을 활성화하는 방법](https://help.directcloud.net/admin_manual/undefined-4/directcloud-shield-irm)에서 SHIELD를 사용하지 않는 것으로 설정되어 있는 경우, 해당 폴더에서는 DirectCloud-SHIELD에 의한 처리가 수행되지 않습니다.
*   상태를 비활성으로 설정하면 라벨이 '보안등급 없음'으로 변경되고, 작업 제한은 해제됩니다.

    한 번 '보안등급 없음' 라벨로 변경되면, 관리자 페이지에서 다시 상태를 활성으로 설정하더라도 '보안등급 없음' 라벨을 원래대로 되돌릴 수는 없습니다.

    단, [파일의 보안등급을 변경하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-7), [사용자 페이지에서 파일의 보안등급을 변경하는 방법](https://help.directcloud.net/user_manual/undefined-3/undefined-4)을 통해 보안등급을 다시 수정하실 수는 있습니다.

### 절차

{% hint style="info" %}
**DirectCloud-SHIELD IRM을 활성화하기**
{% endhint %}

1. 'SHIELD' > '설정' 메뉴를 선택하고, '보안 문서 정의' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (271).png" alt=""><figcaption></figcaption></figure>

2. '보안문서 관리'에서 '사용'을 선택하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2374).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**속성 정의에서 문서의 판정 기준을 추가합니다.**
{% endhint %}

**문서 속성 생성을 시작합니다.**

1. 속성정의 탭을 클릭하고 '속성 추가' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (273).png" alt=""><figcaption></figcaption></figure>

2. 문서 속명에 생성할 판정 기준의 이름을 입력하고, 할당할 보안등급 선택합니다. 상태는  On 으로 설정합니다.

<figure><img src="../../.gitbook/assets/image (274).png" alt=""><figcaption></figcaption></figure>



**문서 내 텍스트에 포함된 개인 정보를 보안등급의 판정 기준으로 설정합니다.**

1. 문서 내 텍스트에 포함된 개인 정보를 보안 문서의 판정 기준으로 사용할 경우, '검출 대상'의 문서 내 개인 정보에서 대상 항목에 체크를 합니다.

<figure><img src="../../.gitbook/assets/image (275).png" alt=""><figcaption></figcaption></figure>

2. 문서 내 개인 정보를 여러 항목 선택한 경우, 활성화된 AND, OR 버튼을 클릭하여 보안 문서의 판정 조건을 변경하실 수 있습니다.\
   \
   OR: 선택한 개인 정보 중 하나라도 문서 내 텍스트에 포함된 경우\
   AND: 선택한 개인 정보가 모두 문서 내 텍스트에 포함된 경우

<figure><img src="../../.gitbook/assets/image (277).png" alt=""><figcaption></figcaption></figure>

3. 선택한 개인 정보가 문서 내 텍스트에 지정한 수 이상 포함된 경우 보안 문서로 판정하려면, '검출 횟수 지정'에 체크하고 숫자를 입력합니다.

<figure><img src="../../.gitbook/assets/image (278).png" alt=""><figcaption></figcaption></figure>



**문서 내 텍스트 또는 파일명에 포함된 단어를 보안등급의 판정 기준으로 설정합니다.**

1. 문서 내 텍스트 또는 파일명에 포함된 단어를 보안 문서의 판정 기준으로 사용할 경우, 검출 대상의 '특정 단어'에서 본문, 파일명 중 하나 또는 둘 다에 체크합니다.

<figure><img src="../../.gitbook/assets/image (279).png" alt=""><figcaption></figcaption></figure>

2. 텍스트 박스에 단어를 입력하고 Enter 키를 누릅니다.\
   여러 단어를 계속 입력할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (280).png" alt=""><figcaption></figcaption></figure>

3. 텍스트 박스에 여러 단어를 입력한 경우, 활성화된 AND, OR 버튼을 클릭하여 보안 문서의 판정 조건을 변경할 수 있습니다.\
   \
   OR: 선택한 개인 정보 중 하나라도 문서 내 텍스트에 포함된 경우\
   AND: 선택한 개인 정보가 모두 문서 내 텍스트에 포함된 경우

<figure><img src="../../.gitbook/assets/image (281).png" alt=""><figcaption></figcaption></figure>

4. '본문'에 체크한 경우, 검출 횟수 설정에 체크하고, 2단계에서 입력한 단어가 문서 내 텍스트에 몇 회 이상 포함되었을 때 보안 문서로 판정할지 횟수를 지정합니다.

<figure><img src="../../.gitbook/assets/image (282).png" alt=""><figcaption></figcaption></figure>



**파일의 확장자를 보안등급의 판정 기준으로 설정합니다.**

1. 파일의 확장자를 보안 문서의 판정 기준으로 사용할 경우, 검출 대상의 확장자에서 대상 확장자에 체크합니다.

<figure><img src="../../.gitbook/assets/image (2363).png" alt="" width="563"><figcaption></figcaption></figure>



**여러 검출 대상의 판정 조건을 설정합니다.**

여러 검출 대상이 설정된 경우, 판정 조건에서 보안 문서의 판정 조건을 설정할 수 있습니다.\
연산자에는 우선순위가 없으므로 왼쪽 조건부터 순서대로 처리됩니다.

1. 좌우의 검출 대상이 모두 판정 조건을 만족했을 때 파일을 보안 문서로 판단하려는 경우에는 OR 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2365).png" alt=""><figcaption></figcaption></figure>

&#x20;       버튼이 AND 버튼으로 변합니다.&#x20;

2. 좌우의 검출 대상 중 어느 한쪽이 판정 조건을 만족했을 때 파일을 보안 문서로 판정하려는 경우에는 AND 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2369).png" alt=""><figcaption></figcaption></figure>

&#x20;      버튼이 OR 버튼으로 변합니다.



**설정한 문서 속성을 등록합니다.**

1. 등록 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2370).png" alt=""><figcaption></figcaption></figure>

2. 속성 정의에 등록한 속성이 추가됩니다.

<figure><img src="../../.gitbook/assets/image (2371).png" alt=""><figcaption></figcaption></figure>

&#x20;     '보안문서 정의' 탭을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2372).png" alt=""><figcaption></figcaption></figure>

3. 보안문서 정의 화면에서, 등록한 속성명이 설정한 보안등급의 문서 속성 항목에 추가되어 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2373).png" alt=""><figcaption></figcaption></figure>
