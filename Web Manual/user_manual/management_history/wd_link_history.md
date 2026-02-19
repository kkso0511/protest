---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/management_history/wd_link_history
---

# \[Web, Drive] 사용자 페이지에서 Link History를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 사용자 페이지의 Link History 메뉴에서 생성된 링크 목록을 표시하고, 각 링크 내역의 상세 정보를 확인하는 절차에 대해 설명합니다.\
또한 Link History에서 링크 생성 화면을 열어 아직 전송되지 않은 링크의 설정 내용을 수정하고 전송하는 방법에 대해서도 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* [특정 그룹이나 사용자에게 공유 링크 사용을 허용하지 않도록 설정하는 방법](https://help.directcloud.net/admin_manual/security_policy/link_restriction)의 절차에 따라 링크에 체크된 권한 세트가 그룹과 사용자에게 부여되어 있어야 합니다.
* Guest 기능 제한에서 Guest가 링크를 생성하지 못하도록 설정된 경우, 아래의 메뉴와 탭은 표시되지 않습니다.\
  자세한 내용은 [Guest의 링크 생성 가능 여부를 설정하는 방법](https://help.directcloud.net/admin_manual/user/guest_link_permission)을 참조해주시기 바랍니다.
  * Web 브라우저\
    사용자 페이지의 Link History 메뉴
  * DirectCloud 드라이브\
    설정 화면의 Link History 탭
* 이미 생성된 링크가 삭제된 경우에도 링크 내역의 상세 정보는 확인할 수 있습니다.
* Link History는 정렬할 수 없습니다.
* DirectCloud 드라이브에서는 전송된 링크를 삭제할 수 없습니다.\
  아래 방법 중 하나로 링크를 삭제해야 합니다.
  * 사용자가 생성한 링크를 삭제하는 방법의 절차에 따라 관리자가 링크를 삭제
  *   Web 브라우저에서 링크를 삭제

      1\. 작업 표시줄의 DirectCloud 드라이브 아이콘을 클릭\
      2\. Web으로 이동 버튼을 클릭하여 Web 브라우저를 표시\
      3\. 본 매뉴얼의 Web 브라우저에서 Link History를 확인하는 방법 > Link History에서 링크를 전송하는 절차에 따라 링크 생성 화면을 표시\
      4\. 오른쪽 아래에 있는 삭제 버튼을 클릭

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 Linki History 확인**
{% endhint %}

**\[링크 내역 보기]**

1. 사용자 페이지에서 Link History 메뉴를 클릭합니다.\
   링크의 기록이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2484).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="162">항목</th><th>설명</th></tr></thead><tbody><tr><td>파일명</td><td>링크가 생성된 폴더 또는 파일의 이름이 표시됩니다.<br>또한 그 아래에는 링크가 생성된 폴더 또는 파일이 저장된 폴더 경로가 표시됩니다.<br>폴더 경로를 클릭하면 링크의 원본 폴더 또는 파일이 저장된 폴더로 이동합니다.</td></tr><tr><td>링크</td><td>링크의 URL이 표시됩니다.<br>../ 는 https://link.directcloud.net 로 대체되어 표시됩니다.</td></tr><tr><td>날짜</td><td>링크가 조작된 날짜와 시간이 표시됩니다.</td></tr><tr><td>Event</td><td><p>작업 링크에 대해 수행된 작업 내용이 표시됩니다.<br>작업의 종류는 아래와 같습니다.</p><p></p><ul><li>생성: 링크 생성</li><li>편집: 링크 편집</li><li>웹메일 발송: 링크를 이메일로 전송</li><li>업로드: 발신자가 링크의 수신 화면에 파일을 업로드</li><li>URL 변경: 링크 URL 변경</li><li>삭제: 링크 삭제</li></ul></td></tr></tbody></table>



2. 자세한 내용을 보려면 파일명을 클릭합니다.\
   링크 내역 세부사항 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2486).png" alt=""><figcaption></figcaption></figure>



3. 링크 기록의 세부정보를 확인합니다.

<table><thead><tr><th width="176">항목</th><th>설명</th></tr></thead><tbody><tr><td>Link URL</td><td>링크 URL, 폴더 이름 또는 파일 이름이 표시됩니다. 파일의 경우 파일 크기가 표시됩니다.</td></tr><tr><td>이벤트(일시)</td><td>링크와 관련된 조작 내용과 조작된 날짜와 시간이 표시됩니다.</td></tr><tr><td>링크 옵션</td><td>[자세히 보기▼]를 클릭하면 링크의 옵션 설정이 표시됩니다.</td></tr><tr><td>웹메일</td><td>이메일로 링크를 보내면 보낸사람, 받는사람, 제목, 내용 등의 정보가 표시됩니다.</td></tr><tr><td>읽기 내역</td><td><p>파일에 접근이 있었던 날짜와 시간, IP 주소, 작업 내역이 표시됩니다.<br>세부 내용은 아래와 같습니다.</p><ul><li>메일 주소:<br><a href="https://help.directcloud.net/user_manual/file_share/wd_link_share">[Web, Drive] 링크를 생성해 공유하는방법</a>에서 수신자 확인에 체크한 경우 메일 주소가 표시됩니다.</li><li>날짜와 시간:<br>링크에 접근한 날짜와 시간이 표시됩니다.</li><li>IP 주소:<br>접근한 측의 IP 주소가 표시됩니다.</li><li>작업 내역:<br>링크 수신 화면에서 사용자가 작업을 수행한 경우, 미리보기, 다운로드, 업로드 중 하나가 표시됩니다.</li></ul></td></tr></tbody></table>



**\[링크 기록에서 링크 보내기]**

1. 사용자 페이지에서 링크 기록 메뉴를 클릭합니다.\
   링크의 기록이 표시됩니다.
2. 링크 설정 방법을 확인하고자 하는 링크 히스토리의 오른쪽 가장자리에 표시되는 링크 버튼을 클릭합니다.\
   링크 만들기 화면이 표시됩니다.
3. 링크 설정 정보를 확인합니다.\
   작성된 후에 전송되지 않은 링크의 경우 설정 내용을 수정하여 전송할 수 있습니다.\
   설정 항목에 대한 자세한 내용은 [\[Web\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/w_link_check)을 참조하십시오.



{% hint style="warning" %}
**DirectCloud 드라이브에서 Link History 확인**
{% endhint %}

**\[링크 내역 보기]**

1. 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭합니다.\
   DirectCloud 드라이브 설정 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (2487).png" alt=""><figcaption></figcaption></figure>



2.  '링크 이력'을 클릭합니다.\
    '링크 이력'에는 다음 정보가 표시됩니다.<br>

    <figure><img src="../../.gitbook/assets/image (2488).png" alt="" width="563"><figcaption></figcaption></figure>

* 링크가 생성된 폴더 이름 또는 파일 이름
* 폴더 경로
* 링크 URL
* 링크 조작 내용



3.  자세한 내용을 보려는 링크 기록의 링크 URL을 클릭합니다.\
    링크 기록의 세부 정보가 표시됩니다.\
    <br>

    <figure><img src="../../.gitbook/assets/image (2489).png" alt="" width="563"><figcaption></figcaption></figure>



4.  링크 기록의 세부정보를 확인합니다.\
    <br>

    <figure><img src="../../.gitbook/assets/image (2490).png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="176">항목</th><th>설명</th></tr></thead><tbody><tr><td>Link URL</td><td>링크 URL, 폴더 이름 또는 파일 이름이 표시됩니다. 파일의 경우 파일 크기가 표시됩니다.</td></tr><tr><td>이벤트(일시)</td><td>링크와 관련된 조작 내용과 조작된 날짜와 시간이 표시됩니다.</td></tr><tr><td>링크 옵션</td><td>[자세히 보기▼]를 클릭하면 링크의 옵션 설정이 표시됩니다.</td></tr><tr><td>웹메일</td><td>이메일로 링크를 보내면 보낸사람, 받는사람, 제목, 내용 등의 정보가 표시됩니다.</td></tr><tr><td>읽기 내역</td><td><p>파일에 접근이 있었던 날짜와 시간, IP 주소, 작업 내역이 표시됩니다.<br>세부 내용은 아래와 같습니다.</p><ul><li>메일 주소:<br><a href="https://help.directcloud.net/user_manual/file_share/wd_link_share">[Web, Drive] 링크를 생성해 공유하는방법</a>에서 수신자 확인에 체크한 경우 메일 주소가 표시됩니다.</li><li>날짜와 시간:<br>링크에 접근한 날짜와 시간이 표시됩니다.</li><li>IP 주소:<br>접근한 측의 IP 주소가 표시됩니다.</li><li>작업 내역:<br>링크 수신 화면에서 사용자가 작업을 수행한 경우, 미리보기, 다운로드, 업로드 중 하나가 표시됩니다.</li></ul></td></tr></tbody></table>



**\[링크 내역에서 미리보기를보고 링크를 만들고 보냅니다.]**

DirectCloud 드라이브의 경우 링크 기록에서 전송되지 않은 링크를 보낼 수 없습니다.\
그러나 파일의 경우 다음 단계를 사용하여 링크 기록에서 미리보기를 보고 링크를 다시 만들고 제출할 수 있습니다.

1. 사용자 페이지에서 링크 기록 메뉴를 클릭합니다.\
   링크의 기록이 표시됩니다.
2. 파일 이름을 클릭합니다.\
   파일 미리보기가 표시됩니다.
3. 링크 만들기 버튼을 클릭합니다.\
   새롭게 링크가 작성되어 '링크 생성' 화면이 표시됩니다.\
   설정 항목에 대한 자세한 내용은 [\[Dirve\] 링크 생성 화면을 표시하여 기본 기능을 확인하는 방법](https://help.directcloud.net/user_manual/file_share/d_link_check)을 참조하십시오.
