---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-3/undefined-14
---

# 메일 서버의 필터에 등록된 메일 주소를 관리 페이지에서 해제하는 방법

### 개요 <a href="#a03" id="a03"></a>

알림 조건을 충족하고 있음에도 알림 메일이 수신되지 않는 경우의 대처 방법의 'Amazon SES의 필터에 등록됨'에 기재된 바와 같이, Amazon SES로의 바운스 메일이 많아지면 사용자의 메일 주소가 DirectCloud의 필터에 등록되는 경우가 있습니다.\
이 매뉴얼에서는, 관리 페이지에서 Amazon SES의 필터를 해제하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '계정 관리'를 사용할 수 있습니다.
* 메일 주소가 필터에 등록된 사용자의 ID와 비밀번호로 사용자 페이지에 로그인한 후, '설정' 화면에서 '본인 확인용 메일 발송' 버튼을 클릭하면 필터를 해제할 수도 있습니다.
* 아래의 경우에는 '등록 메일 주소의 본인 확인' 화면에 접근하면, '무효가 된 URL입니다.'라고 표시됩니다.
  * 본인 확인용 URL이 이미 사용된 경우
  * '등록 메일 주소의 본인 확인' 화면에서 본인 확인이 완료되지 않은 상태에서, 사용자 페이지의 '설정' 화면에서 다시 '본인 확인용 메일 발송' 버튼을 클릭한 경우
  * 본인 확인용 URL의 유효 기간이 만료된 경우

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**'계정 관리' 설정을 표시하기**
{% endhint %}

1. '계정 관리' > '사용자' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**본인 확인용 메일을 발송하기**
{% endhint %}

1. '계정 관리'에서 메일 주소를 활성화하려는 사용자의 편집 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>



2. '사용자 변경' 화면이 표시됩니다.\
   이메일 주소가 비활성화된 경우, 메일 주소 아래에 '이메일 주소 비활성화 안내' 항목이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>



3. '본인 확인 이메일 전송' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>



4. 사용자에게 본인 확인용 메일이 발송됩니다.

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**메일 주소를 활성화하기**
{% endhint %}

이 매뉴얼에서는, 사용자 메일 주소로 수신된 알림 메일에 포함된 본인 확인용 URL을 클릭하여 메일 주소를 활성화하는 절차에 대해 설명합니다.

1. '본인 확인을 위한 이메일입니다.'라는 제목의 알림 메일을 열고, '본인 확인 URL'의 링크를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>



2. 메일 주소의 본인 확인이 완료되어, 메일 주소가 활성화됩니다.\
   '이메일 주소 본인 확인' 화면이 표시됩니다.\
   '설정 화면으로 이동' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>



3. 사용자 페이지의 '설정' 화면이 표시됩니다.\
   로그인 화면이 표시된 경우에는, 사용자의 ID와 비밀번호로 사용자 페이지에 로그인해 주십시오.

<figure><img src="../../.gitbook/assets/image (12).png" alt="" width="335"><figcaption></figcaption></figure>



4. 본인 확인이 완료된 메일 주소가 표시되어 있는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (13).png" alt="" width="375"><figcaption></figcaption></figure>
