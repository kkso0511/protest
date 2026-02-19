---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/directcloud-shield-irm/export_file_usage
---

# 외부로 반출된(다운로드된) 파일의 이용 내역을 확인하는 방법

### 개요

DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM을 계약하신 경우, IRM(Information Rights Management)을 이용하여 의도하지 않은 파일 유출을 방지할 수 있습니다.\
이 매뉴얼 에서는 외부로 반출된 보안문서의 사용 이력을 확인하는 방법을 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 'SHIELD' 항목을 사용 가능합니다.
* 이 매뉴얼 에서 설명하는 DirectCloud-SHIELD IRM은 DirectCloud의 유료 옵션입니다.
* DirectCloud-SHIELD IRM은 다른 유료 옵션인 DirectCloud-SHIELD DLP로 전환할 수 있습니다. 자세한 내용은 DirectCloud 측으로 문의 부탁드립니다.
*   '반출문서 이용내역'에는 다운로드 또는 링크 전송을 통해 외부로 반출된 파일이 표시됩니다.

    Shared Box에서 보안등급 라벨이 부여된 파일 목록을 확인하려면, [파일의 보안등급을 변경하는 방법](https://help.directcloud.net/admin_manual/directcloud-shield-irm/change_security_level)을 참고해주시기 바랍니다.
* 첨부 파일 전송 기능에서는 암호화된 파일을 보낼 수 없습니다.
* '반출문서 이용내역' 메뉴에서는 파일을 미리보기할 수 없습니다.
*   DirectCloud 드라이브에서는 고유 식별 번호가 부여된 파일을 C 드라이브에 캐시 형태로 다운로드한 뒤 열어봅니다. 이는 DirectCloud Storage에서 로컬 PC로 파일을 다운로드하는 것, 즉 외부로 반출하는 것과 동일하게 간주되므로, '반출문서 이용내역'에 파일 열기 로그가 기록됩니다.

    파일을 닫으면 파일 닫기 로그가 기록됩니다.
* 다운로드되는 CSV 파일의 문자 코드는 환경 설정 > 상세 설정 메뉴의 CSV 다운로드 시 문자 코드 설정에서 지정됩니다.\
  자세한 내용은 [다운로드하는CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참고해주시기 바랍니다.

### 절차

{% hint style="warning" %}
**반출된 파일의 사용 이력을 확인하기**
{% endhint %}

1. 'SHIELD' > '반출문서 이용내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2398).png" alt=""><figcaption></figcaption></figure>

2. '반출문서 이용내역'에서 반출된 파일의 사용 이력을 확인합니다.

<figure><img src="../../.gitbook/assets/image (229).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="145.20001220703125">항목</th><th>설명</th></tr></thead><tbody><tr><td>행위</td><td><p>작업 내용이 표시됩니다.<br>다음과 같은 작업이 수행될 때 로그가 기록됩니다.<br></p><ul><li>열기<br>파일을 표시한 경우</li><li>편집<br>파일을 덮어쓰기 저장한 경우</li><li>파일 수정 차단<br>파일의 덮어쓰기 저장이 DirectCloud-SHIELD IRM에 의해 차단된 경우</li><li>다른 이름으로 저장 차단<br>다른 이름으로 파일을 저장하려 할 때 DirectCloud-SHIELD IRM에 의해 차단된 경우</li><li>화면캡처<br>표시 중인 파일을 캡처(스크린샷)한 경우</li><li>화면캡처 차단<br>표시 중인 파일의 캡처(스크린샷) 시도가 DirectCloud-SHIELD IRM에 의해 차단된 경우</li><li>클립보드<br>파일의 텍스트를 복사한 경우</li><li>클립보드 차단<br>파일의 텍스트 복사가 차단된 경우</li><li>인쇄<br>파일을 인쇄한 경우</li><li>인쇄 차단<br>파일 인쇄가 DirectCloud-SHIELD IRM에 의해 차단된 경우</li><li>닫기<br>파일을 닫은 경우</li><li>삭제 처리<br><a href="https://help.directcloud.net/admin_manual/directcloud-shield-irm/delete_export_file">외부로 반출된(다운로드된) 파일을 삭제하는 방법</a>을 통해 파일이 삭제된 경우</li></ul></td></tr><tr><td>파일명/반출번호</td><td>파일 이름과 32자리의 고유 식별 번호가 표시됩니다.<br>다운로드 또는 링크 전송을 통해 외부로 반출되는 파일에는 매번 고유 식별 번호가 부여됩니다.</td></tr><tr><td>보안등급</td><td>파일에 부여된 보안등급 라벨이 표시됩니다.</td></tr><tr><td>사용자</td><td>파일을 조작한 사용자의 이름이 표시됩니다.</td></tr><tr><td>접속아이피</td><td><p>접속한 IP 주소와, <a href="https://help.directcloud.net/admin_manual/security_policy/user_ip_restriction">사용자 페이지에 로그인 가능한 IP 주소를 제한하는 방법</a>에서 허용된 IP 주소인지 여부에 따라 다음 정보가 표시됩니다.</p><ul><li>사내<br>허용된 IP 주소인 경우</li><li>사외<br>허용되지 않은 IP 주소인 경우</li></ul></td></tr><tr><td>날짜</td><td>파일이 조된 날짜와 시간이 표시됩니다.</td></tr><tr><td>크기</td><td>파일의 용량이 표시됩니다.</td></tr></tbody></table>

{% hint style="warning" %}
**반출된 파일의 사용 이력을 필터링 하 확인하기**
{% endhint %}

'반출문서 이용내역'에서는 반출된 파일의 사용 이력을 기간, 사용자, 파일명, 고유 번호, 작업 내용, 건수로 필터링하여 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (228).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="89.20001220703125">No.</th><th>설명</th></tr></thead><tbody><tr><td>1</td><td>계약 시작일부터 현재까지의 반출된 파일 사용 이력을 표시할 기간을 직전 7일, 직전 15일, 직전 1개월, 직전 3개월 중에서 선택합니다.</td></tr><tr><td>2</td><td>계약 시작부터 현재까지의 파일 보안등급 및 암호화 변경 이력을 표시할 기간을 직접 지정합니다.<br>지정할 수 있는 기간은 최대 12개월입니다.</td></tr><tr><td>3</td><td>클릭하여 드롭다운 리스트를 열고, 반출된 파일의 사용 이력을 필터링하여 표시하고자 하는 작업 내용을 선택합니다.</td></tr><tr><td>4</td><td>반출된 파일의 사용 이력을 작업을 수행한 사용자, 파일명, 고유 번호로 필터링하려는 경우, 사용자명 또는 사용자 ID, 파일명, 고유 번호를 입력합니다.</td></tr><tr><td>5</td><td>반출된 파일 사용 이력을 표시할 건수를 10, 25, 50, 100 중에서 선택합니다.</td></tr></tbody></table>

{% hint style="warning" %}
**반출된 파일의 사용 이력을 CSV 파일로 다운로드합니다.**
{% endhint %}

1. '반출문서 이용내역'에서 CSV 다운로드 버튼을 클릭합니다.\
   필요한 경우, 반출된 파일의 사용 이력을 먼저 필터링한 뒤 다운로드하시는 것을 권장합니다.

<figure><img src="../../.gitbook/assets/image (226).png" alt=""><figcaption></figcaption></figure>

2. CSV 파일을 열어 문제가 없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (227).png" alt=""><figcaption></figcaption></figure>
