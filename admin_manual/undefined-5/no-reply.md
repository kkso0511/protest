---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-5/no-reply
---

# no-reply 메일에 회신할 수 있도록 할지 여부를 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 아래 기능에서 전송된 알림 메일의 발신자에는 'no-reply@directcloud.jp'라는 no-reply 메일 주소가 표시됩니다.

* 링크 생성
* 파일첨부 메일발송
* 업로드 요청
* Guest 초대
* Connect User 초대
* 파일별 코멘트

이 매뉴얼에서는, 위 기능으로 수신자에게 전달된 no-reply 메일에 실제로 메일을 전송한 보낸 사람의 메일 주소를 포함하여 회신할 수 있도록 할지 여부를 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지의 '공유 설정' 메뉴를 사용할 수 있습니다.
* 이 매뉴얼의 설정은, 아래 기능으로 전송된 알림 메일만을 대상으로 합니다.\
  그 외 기능으로 전송된 알림 메일은, 회신처 메일 주소가 'no-reply@directcloud.jp'로 고정되기 때문에, 발신자의 메일 주소로 회신할 수 없습니다.
  * 링크 생성
  * 파일첨부 메일발송
  * 업로드 요청
  * Guest 초대
  * Connect User 초대
  * 파일 코멘트
* 이 매뉴얼의 설정과 관계없이, 알림 메일 본문에 있는 '발신자', '초대자', '등록자'에는, 해당 기능을 사용한 사용자의 이름이 표시됩니다.

***

### 절차 <a href="#a04" id="a04"></a>

1. '공유 설정' > '맞춤형 설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2537).png" alt=""><figcaption></figcaption></figure>



2. 'no-reply 메일 회신 설정'에서, 'no-reply 메일 회신'의 '사용' 또는 '사용 안함'을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2538).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="190">항목</th><th>설명</th></tr></thead><tbody><tr><td>사용</td><td>수신자에게 도착한 메일에는 '사용자 이름no-reply@directcloud.jp<br>'와 같이 표시되지만, 회신 시에는 실제로 DirectCloud 기능을 사용하여 메일을 발송한 사용자의 메일 주소가 설정됩니다.</td></tr><tr><td>사용 안함</td><td>no-reply 메일에 회신할 수 없게 됩니다.<br>회신처는 'DirectCloudno-reply@directcloud.co.jp<br>'로 고정되기 때문에, 메일에 회신하더라도 발송한 사용자에게는 전달되지 않습니다.</td></tr></tbody></table>



3. '저장' 버튼을 클릭 합니다.

<figure><img src="../../.gitbook/assets/image (2539).png" alt=""><figcaption></figcaption></figure>
