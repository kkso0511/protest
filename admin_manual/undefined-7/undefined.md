---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-7/undefined
---

# 워크플로우를 활성화하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 워크플로우를 이용하면 사용자가 다음 작업을 수행할 때 결재자의 승인을 받도록 설정할 수 있습니다.

* 파일 다운로드
* 폴더 및 파일 링크 생성
* 파일 첨부 메일 발송
* 파일 업로드

워크플로우의 신청자로 지정된 사용자가 해당 기능을 이용하기 위해 승인 신청을 하고, 워크플로우의 결재자로 지정된 사용자가 이를 승인해야만 작업을 수행할 수 있는 구조입니다.

이 매뉴얼에서는 '워크플로우' > '기본 설정' 메뉴에서 워크플로우를 활성화하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '워크플로우' 항목을 사용할 수 있습니다.
* 이 매뉴얼의 절차로 워크플로우가 활성화되어 있더라도, [특정 폴더에서 워크플로우를 사용하도록 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-20)에서 워크플로우 설정이 사용하지 않음으로 되어 있는 경우, 선택한 폴더에서는 워크플로우를 사용할 수 없습니다.
*   워크플로우의 작성자에는 LDAP 연동 및 SAML 연동으로 불러온 사용자도 추가할 수 있습니다.

    Guest와 Connect User는 추가할 수 없습니다.
* 워크플로우에 포함되지 않은 사용자에 대한 기능 제한은 접근 권한보다 우선합니다.
* 워크플로우에 포함되지 않은 사용자에 대해 일부 기능만 제한하는 설정은 할 수 없습니다.
* 워크플로우의 기본 설정에서 기능의 '다운로드'에 체크를 하면, '보안 정책' ＞ '모바일 보안'메뉴의 이미지 저장, 메일로 전송, 다음 방법으로 열기, 앱에서 열기, 오프라인 시 접근 설정이 '사용 안함'으로 고정되며, 모바일 애플리케이션에서 ⁝ 버튼을 탭했을 때 이미지 저장, 내보내기, 오프라인으로 이용 가능하게 하기 메뉴가 표시되지 않도록 설정됩니다.
* 다운로드 워크플로우에서 신청자로 추가된 사용자는 폴더 다운로드를 할 수 없게 됩니다.\
  파일을 다운로드하려고 하면 워크플로우 신청 화면이 표시됩니다.
* 업로드 워크플로우에서 신청자로 추가된 사용자는 폴더 업로드를 할 수 없게 됩니다.\
  파일을 업로드하려고 하면 워크플로우 신청 화면이 표시됩니다.
*   다운로드·업로드 워크플로우에서 신청자로 추가된 사용자는 DirectCloud 드라이브에서 다음 작업을 수행할 수 없게 됩니다.

    * 드래그 앤 드롭으로 다운로드 및 업로드
    * 직접 편집
    * 폴더 및 파일 이름 변경
    * 폴더 및 파일 이동
    * 폴더 및 파일 복사
    * 폴더 생성
    * 폴더 및 파일 삭제

    자세한 내용은 [다운로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/undefined-9/undefined-3)과 [업로드 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/undefined-9/undefined-6)을 참고해 주세요.
* 링크 워크플로우를 생성한 경우, 신청자로 지정된 사용자는 링크 복사 및 외부 메일 프로그램을 통한 전송을 할 수 없게 됩니다. 자세한 내용은 [링크전송 워크플로우를 신청하는 방법](https://help.directcloud.net/user_manual/undefined-9/undefined-4)을 참고해 주세요.
* DirectCloud-SHIELD DLP를 계약한 경우, 승인 워크플로우의 적용 대상으로 DLP를 선택할 수 있습니다.
* Warm Storage를 계약한 경우 Warm Storage를 사용할 수 있습니다.
* Cold Storage를 계약한 경우 Cold Storage도 사용할 수 있습니다.
* 하지만 Warm Storage와 Cold Storage에서는 워크플로우를 사용할 수 없으므로 워크플로우의 적용 대상으로 지정할 수 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**워크플로우 활성화**
{% endhint %}

1. '워크플로우' > '설정' 메뉴를 클릭합니다.\
   워크플로우 기본 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2178).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. 워크플로우 기본 설정에서 사용을 선택합니다.\
   워크플로우의 설정 항목이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2179).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

3. 다음 설정을 지정하고 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2180).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="222">항목</th><th>내용</th></tr></thead><tbody><tr><td>적용범위</td><td>워크플로우 설정을 적용할 폴더를 선택합니다.</td></tr><tr><td>기능</td><td>워크플로우를 사용하려는 기능을 선택합니다.<br>'다운로드'를 선택하면 신청자로 설정된 사용자가 파일을 다운로드할 수 있는 기간을 설정할 수 있습니다. 기간을 지정하려면 유효 기간의 사용을 선택하고 다운로드 가능한 일 수로 텍스트 상자에 1에서 365 사이의 숫자를 입력합니다.</td></tr><tr><td>결재선 관리담당자</td><td><p>워크플로우를 만들 수 있는 사용자를 설정합니다.<br>모든 사용자를 설정하는 경우 워크플로우 작성자 추가 절차를 참조하십시오.</p><ul><li>시스템 관리자 모두 포함:<br>계약 담당 관리자 및 일반 관리자</li><li>Shared Box의 각 폴더마스터 모두 포함:<br>마스터, 전체권한의 권한이 부여된 사용자</li></ul></td></tr><tr><td>결재선 편집</td><td><p>생성된 워크플로우를 변경할 수 있는 사용자를 선택합니다.</p><ul><li>대상 워크플로우를 만든 사용자만:<br>워크플로우를 만든 사용자에게만 변경을 허용합니다.</li><li>작성 권한이 부여된 모든 사용자:<br>워크플로우 작성자에 설정된 사용자에게 변경을 허용합니다.</li></ul></td></tr><tr><td>결재선 미지정 사용자</td><td><p>워크플로우의 신청자 이외의 사용자에게 '기능'에서 확인한 기능의 조작을 허용할지 여부를 설정합니다.</p><ul><li>기능을 제한함:<br>작업을 허용하지 않으려면 선택합니다.</li><li>기능을 제한하지 않음:<br>작업을 허용하려면 선택합니다.</li></ul></td></tr></tbody></table>



**\['워크플로우에 포함되지 않은 사용자'에서 '기능 제한함'을 선택한 경우]**

'결재선 미지정 사용자에서 '기능을 제한함'을 선택한 경우 신청자 이외의 사용자가 '다운로드', '링크전송', '파일첨부 메일발송', '업로드' 작업을 시도하면, 아래의 "이 기능을 사용할 권한이 없습니다."라는 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2181).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**워크플로우 결재선 관리담당자 추가**
{% endhint %}

1. 워크플로우 기본 설정 화면에서 워크플로우 '결재선 관리담당자'의 '사용자 추가' 버튼을 클릭합니다.\
   사용자 추가 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2183).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

2. 권한을 부여할 사용자의 이름 또는 ID를 입력하고 검색 버튼을 클릭합니다.\
   검색 결과가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2184).png" alt=""><figcaption></figcaption></figure>

&#x20;     &#x20;

3. 워크플로우 결재선 관리담당자로 추가할 사용자의 추가 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2185).png" alt=""><figcaption></figcaption></figure>

&#x20;     워크플로 결재선 관리담당자에 사용자가 추가됩니다.

<figure><img src="../../.gitbook/assets/image (2186).png" alt=""><figcaption></figcaption></figure>



4. 필요한 경우 사용자추가를 반복하여 워크플로우 결재선 관리담당자로 여러 사용자를 추가합니다.



5. 저장 버튼을 클릭합니다. 워크플로우의 기본 설정이 저장됩니다.

<figure><img src="../../.gitbook/assets/image (2187).png" alt=""><figcaption></figcaption></figure>
