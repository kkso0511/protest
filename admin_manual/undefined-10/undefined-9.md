---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/undefined-10/undefined-9
---

# 업로드용 전용 이메일 주소로 파일을 수신한 기록을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 폴더별로 고유한 업로드 전용 메일 주소를 설정함으로써, 메일에 파일을 첨부하여 파일을 업로드할 수 있습니다. 메일 주소는 DirectCloud에 의해 자동으로 생성됩니다.\
이 매뉴얼에서는, [전용 이메일 주소를 통해 특정 폴더에 파일을 업로드하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-21)에서 생성된 업로드 전용 메일 주소로 수신한 메일의 이력을 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* 업로드 전용 메일 주소로 파일을 업로드할 경우, 하나의 메일에 첨부할 수 있는 파일 수는 최대 100개입니다.
* 하나의 메일에 첨부할 수 있는 파일 크기의 상한은 메일 서버의 설정에 따라 다릅니다.\
  예를 들어 Gmail의 경우, 첨부 파일이 25MB를 초과하면 파일이 Google 드라이브에 업로드되고, 메일에는 Google 드라이브에 업로드된 파일의 링크 URL이 기재됩니다.\
  이 경우 DirectCloud는 첨부 파일을 수신할 수 없기 때문에, '로그 현황' > '업로드용 메일 수신내역' 메뉴의 '업로드 결과'에는 '실패(첨부 파일 누락)'로 기록됩니다.
* 아래의 사유로 파일 업로드에 실패한 경우에는, '업로드용 메일 수신내역'의 '업로드 결과'에 실패 사유가 표시되지 않고, '0/1'과 같이 표시됩니다.\
  이는 '업로드에 성공한 수/메일로 업로드된 파일 수'를 의미합니다.\
  '수신 이력 상세' 화면에서 '업로드' 열의 '실패' 오른쪽에 표시된 i 마크에 커서를 올리면, 업로드에 실패한 사유를 확인할 수 있습니다.
  * [폴더의 용량 제한을 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-4/undefined-18)에서 설정된 용량을 초과한 경우
  * [업로드 가능한 파일의 크기를 제한하는 방법](https://help.directcloud.net/admin_manual/undefined/undefined-2), [업로드 가능한 파일을 확장자로 제한하는 방법](https://help.directcloud.net/admin_manual/undefined/undefined-3)에 따른 설정으로 인해 파일 업로드가 제한된 경우
  * DirectCloud AI가 활성화된 폴더에서 업로드 가능한 파일 수 또는 용량을 초과하여 업로드가 제한된 경우
  * DirectCloud AI가 활성화된 폴더에 확장자가 '.pdf'가 아닌 파일이 업로드되어 업로드가 제한된 경우
* DirectCloud AI가 활성화된 폴더에 파일을 업로드할 때의 제한 사항에 대해서는, [DirectCloud AI를 활용하기 위한 파일을 준비하는 방법](https://help.directcloud.net/user_manual/directcloud-ai/directcloud-ai-1)의 '제한·보충 사항'을 참조해 주십시오.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**업로드용 이메일 수신내역 확인**
{% endhint %}

1. '로그 현황' > '업로드용 이메일 수신내역' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2550).png" alt=""><figcaption></figcaption></figure>



2. 업로드용 이메일 수신내역에서 업로드 전용 이메일 주소의 수신 내역을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2551).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="179.20001220703125">항목</th><th>설명</th></tr></thead><tbody><tr><td>받는 이메일/폴더</td><td><p>업로드 전용 메일 주소 및 유효한 폴더 경로가 표시됩니다.<br>아래의 경우에는 폴더 경로가 아닌 '무효가 된 메일 주소'로 표시됩니다.</p><ul><li>폴더가 이동되거나 삭제된 경우</li><li>파일을 발송하기 전에, <a href="https://help.directcloud.net/admin_manual/undefined-4/undefined-21">전용 이메일 주소를 통해 특정 폴더에 파일을 업로드하는 방법</a>의 절차에서 업로드 전용 메일 주소가 '사용 안함'으로 설정된 경우</li></ul></td></tr><tr><td>날짜</td><td>업로드 전용 메일 주소가 메일을 수신한 일시가 표시됩니다.</td></tr><tr><td>보낸사람</td><td>보낸사람의 메일 주소가 표시됩니다.</td></tr><tr><td>업로드 수</td><td><p>업로드 전용 메일 주소를 통해 정상적으로 업로드된 파일의 수가 표시됩니다.<br>단, 아래의 경우에는 파일 수가 아닌 다른 정보가 표시됩니다.</p><ul><li>메일 주소가 무효가 된 경우：<br>'실패(메일 주소가 무효)'</li><li>첨부 파일이 누락된 경우：<br>'실패(첨부 파일의 누락)'</li><li>첨부 파일이 100개를 초과한 경우：<br>'실패(첨부 파일 개수 상한 초과)'</li></ul></td></tr><tr><td>동작</td><td>버튼을 클릭하면 '수신 이력 상세' 화면이 표시됩니다.<br>자세한 내용은 아래의 '업로드 전용 메일 수신 이력의 상세를 확인하기'를 참조해 주십시오.</td></tr></tbody></table>



{% hint style="warning" %}
**업로드용 이메일 수신내역 세부 정보**
{% endhint %}

1. '업로드용 이메일 수신내역'에서 세부정보를 확인하려는 수신 기록의 '세부 정보' 열에 표시된 버튼을 클릭합니다. '수신내역'화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2552).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. 수신된 이메일 세부정보를 확인합니다.

<figure><img src="../../.gitbook/assets/image (2553).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="169.60003662109375">항목</th><th>설명</th></tr></thead><tbody><tr><td>이메일 주소/폴더</td><td><p>업로드 전용 메일 주소 및 유효한 폴더 경로가 표시됩니다.<br>아래의 경우에는 폴더 경로가 아닌 '무효가 된 메일 주소'로 표시됩니다.</p><ul><li>폴더가 이동되거나 삭제된 경우</li><li>파일을 발송하기 전에, <a href="https://help.directcloud.net/admin_manual/undefined-4/undefined-21">전용 이메일 주소를 통해 특정 폴더에 파일을 업로드하는 방법</a>의 절차에서 업로드 전용 메일 주소가 '사용 안함'으로 설정된 경우</li></ul></td></tr><tr><td>받은 날짜</td><td>업로드 전용 메일 주소가 메일을 수신한 일시가 표시됩니다.</td></tr><tr><td>보낸 사람</td><td>보낸사람의 메일 주소가 표시됩니다.</td></tr><tr><td>수신 파일 정보</td><td><p>수신한 파일의 정보가 표 형식으로 표시됩니다.<br>업로드 실패 사유가 '메일 주소가 무효' '첨부 파일이 누락됨' '첨부 파일이 100개를 초과함' 중 하나에 해당하는 경우에는, 이 정보가 표시되지 않습니다.</p><ul><li>파일 <br>수신한 파일의 이름이 표시됩니다.</li><li>용량 <br>수신한 파일의 용량이 표시됩니다.</li><li>업로드 일시 <br>업로드 전용 메일 주소가 수신한 파일이 폴더에 업로드된 일시가 표시됩니다.</li><li>업로드 <br>파일의 업로드 결과가 표시됩니다.<br>파일 업로드에 실패한 경우에는, 실패 사유를 확인하기 위한 인포메이션 마크가 표시됩니다.</li></ul></td></tr></tbody></table>



3. 업로드용 이메일 수신내역의 세부사항을 CSV 파일로 다운로드하려면, 'CSV 다운로드' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2554).png" alt=""><figcaption></figcaption></figure>



4. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2555).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**수신한 이메일에 대해 자세히 알아보기**
{% endhint %}

1. '수신 내역' 상세화면에서 '받은 메일' 오른쪽에 표시되는 ▼ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2556).png" alt=""><figcaption></figcaption></figure>



2. 이메일 제목과 본문을 확인합니다.

<figure><img src="../../.gitbook/assets/image (2557).png" alt=""><figcaption></figcaption></figure>



3. 수신한 메일을 다운로드하려면 '다운로드' 버튼을 클릭합니다.\
   확장자 'eml' 파일(EML 형식의 파일)로 메일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (2558).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

4. 다운로드한 파일을 열고 문제 없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (2559).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**업로드 전용 메일의 수신 내역을 필터링하여 표시**
{% endhint %}

업로드 전용 메일 수신 내역에서는 업로드 전용 메일의 수신 내역을 기간, 업로드 전용 메일 주소, 발신 메일 주소, 건수로 좁혀 표시할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2560).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="100">No.</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>업로드 전용 메일 수신 이력을 표시할 기간을, '최근 7일' '최근 15일' '최근 1개월' '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작일부터 현재까지의 업로드 전용 메일 수신 이력을 표시할 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>업로드 전용 메일 수신 이력을 업로드 전용 메일 주소 또는 송신처 메일 주소로 필터링하려는 경우, '받는 이메일' 또는 '보낸 사람'을 입력합니다.</td></tr><tr><td>❹</td><td>업로드 전용 메일 수신 이력을 표시할 건수를, '10' '25' '50' '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**업로드 전용 이메일 수신 내역을 CSV 파일로 다운로드 하기**
{% endhint %}

1. '업로드용 이메일 수신 내역'에서 'CSV 다운로드' 버튼을 클릭합니다.\
   CSV 파일이 다운로드됩니다.\
   필요한 경우 수신 내역을 필터링하여 다운로드 하는 것이 좋습니다.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
