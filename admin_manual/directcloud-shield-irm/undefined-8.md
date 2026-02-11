---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/undefined-8
---

# 보안문서 설정을 관리자 페이지에서 해제하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 이용하고 있는 경우,\
IRM(Information Rights Management)을 통해 의도치 않은 파일 유출을 방지할 수 있습니다.\
여기에서는 DirectCloud-SHIELD IRM에서 파일 암호화와 보안등급 라벨을 해제하는 방법에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
* 암호화 문서 목록에는 Shared Box에 저장되어 있는 파일이 표시됩니다.\
  반출된 파일의 목록을 확인하고 싶은 경우에는 [외부로 반출된(다운로드된) 파일의 이용 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined-10)을 참고해주시기 바랍니다.
* [사용자 페이지에서 파일의 보안문서 설정을 해제하는 방법](https://help.directcloud.net/user_manual/undefined-3/undefined-5)을 통해 암호화를 해제할 수도 있습니다.
* 본 매뉴얼의 절차 또는 [사용자 페이지에서 파일의 보안문서 설정을 해제하는 방법](https://help.directcloud.net/user_manual/undefined-3/undefined-5)으로 암호화가 해제되어 보안등급 라벨이 표시되지 않게 된 파일은 암호화 문서 목록에도 표시되지 않습니다.
* [보안문서 판정 기준 설정 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/undefined)에서 상태가 ‘비활성’으로 설정되어 보안등급 라벨이 ‘보안등급 없음’으로 변경된 파일은 암호화 문서 목록에 표시됩니다.

### 절차

{% hint style="info" %}
**보안등급 라벨이 부여된 파일을 확인하기**
{% endhint %}

1. 'SHIELD' > '보안문서 현황' 목록 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (235).png" alt=""><figcaption></figcaption></figure>

2. '보안문서 현황'에서 보안등급 라벨이 부여된 파일의 목록을 확인합니다.

<figure><img src="../../.gitbook/assets/image (236).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="147.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일</td><td>보안등급 라벨이 부여된 파일의 이름이 표시됩니다.</td></tr><tr><td>보안등급</td><td>파일에 부여된 보안등급 라벨이 표시됩니다.</td></tr><tr><td>사용자</td><td>파일을 업로드한 사용자의 이름이 표시됩니다.</td></tr><tr><td>날짜</td><td>파일이 업로드된 일시가 표시됩니다.</td></tr><tr><td>크기</td><td>파일의 용량이 표시됩니다.</td></tr><tr><td>동작</td><td>버튼을 클릭하면 암호화 정보 화면에서 아래 작업을 수행할 수 있습니다.<br>· 파일의 보안등급 변경<br>· 파일 암호화 해제</td></tr></tbody></table>

{% hint style="info" %}
**파일 암호화 해제**
{% endhint %}

1. '보안문서 현황'에서 암호화를 해제 하려는 파일의 동작 열에 있는 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (237).png" alt=""><figcaption></figcaption></figure>

2. '보안문서 해제' 버튼을 클릭 합니다.

<figure><img src="../../.gitbook/assets/image (2390).png" alt=""><figcaption></figcaption></figure>

3. 확인 화면에서 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2391).png" alt="" width="563"><figcaption></figcaption></figure>

4. 파일의 보안등급 라벨과 암호화가 해제되며, 암호화 문서 목록에서 해당 파일이 표시되지 않습니다.

<figure><img src="../../.gitbook/assets/image (2392).png" alt=""><figcaption></figcaption></figure>



