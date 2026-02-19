---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/log/file_usage_history
---

# 사용자의 파일 이용 내역을 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 '로그 현황' > '파일 이용 내역' 메뉴에서 사용자의 작업 내역을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 관리자 권한이 부여된 사용자는 관리자 페이지에서 '로그 현황' 항목에 접근 가능합니다.
* Guest, LDAP 연동 및 SAML 연동으로 취득한 사용자, Connect User의 조작 이력도 기록됩니다.
* 사용자의 조작 이력에는, 파일에 유효 기한을 설정한 로그 및 해제한 로그는 기록되지 않습니다.\
  삭제된 이후의 결과만 기록됩니다.\
  파일의 유효 기한 설정 일시와 삭제 예정 일시를 확인하고 싶은 경우에는, [사용자가 파일에 유효기간을 설정한 내역을 확인하는 방법](https://help.directcloud.net/admin_manual/log/file_expiry_history)을 참조해 주시기 바랍니다.
* 온라인 편집의 경우 파일 이용 내역의 '동작'열에는, 온라인 편집 화면을 실행했을 때의 로그로 '온라인 편집', 파일명을 변경하여 편집 화면을 종료했을 때의 로그로 '덮어쓰기 저장'이 기록됩니다.\
  파일 편집 중에 저장한 시점에는 로그가 기록되지 않습니다.\
  또한, 파일 내용을 변경하지 않고 편집 화면을 종료한 경우나, 코멘트를 추가한 경우에도 로그는 기록되지 않습니다.
* 링크 수신 화면에서 파일이 업로드된 경우에는, '동작'열에 '파일 업로드'로 기록됩니다.\
  또한 '사용자'에는 링크를 생성한 사용자의 이름이 아니라, 파일을 업로드한 사용자가 입력한 이름이 기록됩니다.\
  검색 대상으로 링크를 생성한 사용자의 아이디를 '사용자 ID'로 지정하여 필터링했을 때, '동작'열에 '파일 업로드'로 표시되는 경우에는, '사용자명'에 링크 수신 화면에서 파일을 업로드한 사용자의 이름이 표시됩니다.
* DirectCloud 드라이브에서 이동 대상 폴더에 동일한 이름의 파일을 이동할 때 '파일을 바꾸기'를 선택한 경우, 바뀐 파일은 버전 정보를 포함하여 완전히 삭제되므로, 휴지통으로 이동되지 않습니다.\
  이 경우, 조작 이력의 '액션'에는 '삭제'가 기록되지 않고, '이동'만 기록됩니다.
* 'DirectCloud-CONNECT'를 이용할 수 있는 경우, 사용자의 조작 이력에 Connect 폴더에 관한 조작 로그가 기록됩니다.
* 'DirectCloud-SHIELD DLP'를 계약하고 있는 경우, 사용자의 조작 이력에 DLP 폴더에 관한 조작 로그가 기록됩니다.
* Warm Storage를 이용할 수 있는경우, 사용자의 조작 이력에 Warm Storage 폴더에 관한 조작 로그가 기록됩니다.
* 'Cold Storage'를 계약하고 있는 경우에는, 사용자의 조작 이력에 Cold Storage 폴더에 관한 조작 로그가 기록됩니다.
* Connect User로 초대받은 회사 ID의 경우에는, 사용자의 조작 이력에 초대한 측 사용자의 조작 이력은 기록되지 않습니다.
* 다운로드되는 CSV 파일의 문자 코드는, '공유 설정' > '세부 기능 설정' 메뉴의 '문자 인코딩'에서 설정되어 있습니다.\
  자세한 내용은, [다운로드하는 CSV 파일의 문자 코드를 설정하는 방법](https://help.directcloud.net/admin_manual/detail_settings/csv_encoding)을 참조해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**사용자의 파일 이용 내역 확인**
{% endhint %}

**\[표시 순서]**

1. '로그 현황' > '파일 이용 내역' 메뉴를 클릭하십시오.

<figure><img src="../../.gitbook/assets/image (1494).png" alt=""><figcaption></figcaption></figure>



2. 사용자의 작업 내역을 확인합니다.\
   Connect User를 초대하면 회사 사용자 외에도 Connect User의 작업 내역이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1495).png" alt=""><figcaption></figcaption></figure>



**\[파일 이용 내역 항목]**

| 항목     | 설명                                                                                                                                                                                                                                                                                                                                                                     |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 동작     | <p>사용자가 수행한 작업이 표시됩니다.<br>동작 유형에 대한 자세한 내용은 하단의 <strong>동작</strong> 표를 참조하십시오.<br>또한 17가지 유형의 Connect User 동작에 대한 자세한 내용은 <strong>Connect User 동작</strong> 의 표를 참조하십시오.</p>                                                                                                                                                                                            |
| 파일/폴더명 | <p>사용자가 조작한 폴더 및 파일이 표시됩니다.</p><ul><li>'동작'이 'My Box 파일 자동 삭제'인 경우에는, 폴더 경로의 맨 앞에 사용자 ID가 표시됩니다.</li><li>'동작'이 '이름 변경'인 경우에는, 변경 후 이름, 저장된 폴더 경로, 변경 전 이름이 표시됩니다.</li><li>'동작'이 '복사'인 경우에는, 복사 대상 파일 또는 폴더의 이름, 복사 대상 폴더 경로, 복사 원본 폴더 경로가 표시됩니다.</li><li>'동작'이 '이동', '자동 이동', '자동 이동(EML 파일)'인 경우에는, 이동 대상 파일 또는 폴더의 이름, 이동 대상 폴더 경로, 이동 원본 폴더 경로가 표시됩니다.</li></ul>    |
| 사용자    | <p>조작한 사용자의 이름이 표시됩니다.<br>이름에 마우스 커서를 올리면, 툴팁으로 사용자 ID를 확인할 수 있습니다.</p>                                                                                                                                                                                                                                                                                                |
| 기기     | <p>조작 시 사용한 기기에 따라 아이콘이 표시됩니다.<br></p><p><strong>NOTE:</strong><br>모바일 환경(모바일 Web 브라우저 어플리케이션, iOS 애플리케이션, Android 애플리케이션)에서 로그인한 경우에는, 모바일 아이콘이 표시됩니다.<br></p><p>아이콘에 커서를 올리면, 툴팁에 아래 정보가 표시됩니다.</p><ul><li>PC Web 브라우저, 모바일 Web 브라우저:<br>Web 브라우저</li><li>PC Agent, DirectCloud 드라이브:<br>컴퓨터명</li><li>iOS 애플리케이션:<br>기기명</li><li>Android 애플리케이션:<br>기기 모델명</li></ul> |
| 접속 아이피 | <p>연결할 IP 주소와 <a href="https://help.directcloud.net/admin_manual/security_policy/user_ip_restriction">사용자 페이지에 로그인할 수 있는 IP 주소를 제한하는 방법</a>으로 허용된 IP 주소인지 여부에 따라 다음 정보 중 하나가 표시됩니다.</p><ul><li>허용된 IP 주소의 경우:<br>사내</li><li>허용되지 않는 IP 주소의 경우:<br>사외</li></ul>                                                                                                         |
| 날짜     | 사용자가 조작한 날짜와 시간이 표시됩니다.                                                                                                                                                                                                                                                                                                                                                |
| 크기     | 사용자가 조작한 파일의 용량이 표시됩니다.                                                                                                                                                                                                                                                                                                                                                |



**\[동작]**

<table><thead><tr><th width="226.4000244140625">동작작</th><th width="528.800048828125">설명</th></tr></thead><tbody><tr><td>파일 업로드</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage의 폴더에 파일을 업로드</li><li>사용자 API의 '파일 업로드' 실행</li></ul></td></tr><tr><td>업데이트</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage의 폴더에 파일을 업로드한 후, 덮어쓰기 저장</li><li>파일의 내용을 변경하고 온라인 편집 화면을 종료</li></ul></td></tr><tr><td>폴더 만들기</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage의 폴더에서 폴더를 생성</li><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage의 폴더에 폴더를 업로드</li><li>사용자 API의 "폴더 추가" 수행</li></ul></td></tr><tr><td>EML 폴더 자동 생성</td><td>DirectCloud AI의 'AI 요약'이 활성화된 폴더에서, 요약 및 벡터 데이터 생성이 완료된 EML 파일을 자동 이동하기 위한 'EML' 폴더를 자동으로 생성합니다.</td></tr><tr><td>이름 변경</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage의 폴더에서, 폴더 또는 파일의 이름을 변경</li><li>사용자 API의 '폴더명 변경', '파일명 변경'을 실행</li></ul></td></tr><tr><td>이동</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage의 폴더에서, 폴더 또는 파일을 이동</li><li>Shared Box의 고스트에서 '이동으로 가져오'를 실행</li><li>Cold Storage 내에서 폴더 또는 파일을 이동</li><li>사용자 API의 '폴더 이동', '파일 이동'을 실행</li></ul></td></tr><tr><td>자동 이동</td><td>폴더 속성 기능으로 설정된 Shared Box에서 Warm Storage 또는 Cold Storage로 파일의 자동 이동을 실행<br><br><strong>NOTE</strong>:<br>이동된 각 파일마다 조작 이력이 기록됩니다.<br>폴더는 '자동 이동'으로 기록되지 않습니다.</td></tr><tr><td>자동 이동(EML 파일)</td><td>DirectCloud AI의 'AI 요약'이 활성화된 폴더에서, 요약 및 벡터 데이터 생성이 완료된 EML 파일을 'EML' 폴더로 자동 이동합니다.</td></tr><tr><td>파일 자동 변환</td><td>DirectCloud AI의 'AI 요약'이 활성화된 폴더에서, EML 파일의 요약 내용을 텍스트 파일로 저장합니다.</td></tr><tr><td>복사</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더에서 폴더 또는 파일을 복사</li><li>Shared Box의 고스트에서 '복사로 가져오기'를 실행</li></ul></td></tr><tr><td>해동 요청</td><td>Cold Storage에서 Shared Box로 파일 복원을 요청</td></tr><tr><td>해동</td><td>Cold Storage에서 Shared Box로 파일 복원</td></tr><tr><td>이전 버전 복원</td><td>My Box, Shared Box, Connect 폴더, DLP 폴더의 파일을 이전 버전으로 복원</td></tr><tr><td>휴지통 복구</td><td>휴지통의 'My Box / Shared Box', 'Connect', 'DLP', 'Warm Storage', 'Cold Storage'에서 폴더 또는 파일을 복원</td></tr><tr><td>삭제</td><td>사용자 휴지통이 '사용 안함'으로 설정되어 있는 경우에, My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage에서 폴더 또는 파일을 삭제</td></tr><tr><td>자동삭제 (파일 기한)</td><td>파일 기한 기능으로 설정된, My Box, Shared Box, Connect 폴더, DLP 폴더의 파일을 자동으로 삭제합니다.</td></tr><tr><td>자동삭제 (My Box)</td><td>My Box 파일의 자동 삭제를 실행</td></tr><tr><td>자동삭제 (폴더옵션)</td><td><p>폴더 옵션 기능으로 설정된 Shared Box, Connect 폴더, DLP 폴더의 폴더 또는 파일을 자동으로 삭제합니다.</p><p></p><p><strong>NOTE</strong>:<br>삭제된 파일 및 폴더 각각에 대해 조작 이력이 기록됩니다.</p></td></tr><tr><td>휴지통</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage 폴더, Cold Storage 폴더에서 폴더 또는 파일을 삭제(휴지통으로 이동)</li><li>Connect 폴더의 폴더·파일을 삭제하여, 휴지통 'Connect'로 이동</li><li>DLP 폴더의 폴더·파일을 삭제하여, 휴지통 'DLP'로 이동</li><li>Warm Storage 폴더의 폴더·파일을 삭제하여, 휴지통 'Warm Storage'로 이동</li><li>Cold Storage 폴더의 폴더·파일을 삭제하여, 휴지통 'Cold Storage'로 이동</li><li>사용자 API의 '폴더 삭제', '파일 삭제'를 실행</li></ul></td></tr><tr><td>이동 취소</td><td><p>폴더 또는 파일의 이동을 취소</p><p></p><p><strong>NOTE</strong>:<br>Warm Storage 또는 Cold Storage에서는 이동을 취소할 수 없습니다.</p></td></tr><tr><td>복사 취소</td><td>폴더 또는 파일의 복사를 취소</td></tr><tr><td>삭제 취소</td><td><p>사용자 휴지통이 '사용 안함'으로 설정되어 있는 경우에, My Box, Shared Box, Connect 폴더, DLP 폴더에서 폴더 또는 파일의 삭제를 취소</p><p></p><p><strong>NOTE</strong>:<br>Warm Storage 및 Cold Storage의 폴더에서는 삭제를 취소할 수 없습니다.</p></td></tr><tr><td>휴지통 취소</td><td><p>My Box, Shared Box, Connect 폴더, DLP 폴더에서, 폴더 또는 파일의 삭제(휴지통으로 이동)를 취소</p><p></p><p><strong>NOTE</strong>:<br>Warm Storage 또는 Cold Storage에서는, 휴지통으로의 이동을 취소할 수 없습니다.</p></td></tr><tr><td>온라인 편집</td><td>온라인 편집 화면을 표시</td></tr><tr><td>AI 데이터 편집</td><td>DirectCloud AI가 활성화된 폴더에서, 데이터 청크를 편집하거나 삭제하여 저장</td></tr><tr><td>문서 속성 편집</td><td>미리보기 화면에서, 문서 속성 정보를 변경</td></tr><tr><td>문서 속성 다운로드</td><td><ul><li>미리보기 화면에서, 문서 속성 정보를 다운로드</li><li>문서 속성 검색 결과에서, 문서 속성 정보를 다운로드</li></ul></td></tr><tr><td>파일 정보 다운로드</td><td>'문서 관리' 폴더에서, 선택한 여러 파일의 문서 속성을 다운로드</td></tr><tr><td>미리보기</td><td><ul><li>My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage의 폴더에서 파일을 미리보기</li><li>사용자 API의 '파일 뷰어 생성'을 실행</li></ul></td></tr><tr><td>DirectCloud 드라이브에서 열기</td><td><p></p><ul><li>DirectCloud 드라이브에서 파일을 직접 탐색</li><li>Windows 탐색기에서 DirectCloud 드라이브의 파일 표시 방법 변경(축소판 이미지 크기, 미리보기 표시 등)</li></ul></td></tr><tr><td>Drive 오프라인 폴더로 다운로드</td><td>My Box 또는 Shared Box의 폴더에 있는 파일을, DirectCloud 드라이브의 오프라인 폴더에 저장</td></tr><tr><td>다운로드</td><td><ul><li>My Box, Shared Box, 문서 관리 폴더, Connect 폴더, DLP 폴더, Warm Storage의 폴더에서 파일을 다운로드</li><li>사용자 API의 '파일 다운로드'를 실행</li></ul></td></tr><tr><td>파일첨부 메일발송</td><td>파일첨부 메일발송 기능으로 파일을 전송</td></tr><tr><td>mobile 메일에 파일 첨</td><td>모바일 애플리케이션의 '다운로드' > '메일로 전송'을 선택</td></tr><tr><td>다른 앱에 파일 첨부</td><td><p>모바일 애플리케이션에서, 아래를 선택</p><ul><li>'다운로드' > '다음 방법으로 열기'</li><li>'다운로드' > '다음 앱으로 열기'를 선택</li></ul><p></p><p><strong>NOTE</strong>:<br>버전 3.4.0까지의 모바일 애플리케이션을 사용하고 있는 경우에 기록됩니다.</p></td></tr><tr><td>다른 앱으로 열기</td><td><p>모바일 애플리케이션(iOS, Android)의 '다운로드' > '다른 앱으로 열기'를 선택</p><p></p><p><strong>NOTE</strong>:<br>버전 3.5.0 이후의 모바일 애플리케이션을 사용하고 있는 경우에 기록됩니다.</p></td></tr><tr><td>다른 앱으로 보내기</td><td><p>모바일 애플리케이션(Android)의 '다운로드' > '다른 앱으로 보내기'를 선택</p><p></p><p><strong>NOTE</strong>:<br>버전 3.5.0 이후의 모바일 애플리케이션을 사용하고 있는 경우에 기록됩니다.</p></td></tr><tr><td>링크 생성</td><td><ul><li>My Box, Shared Box, DLP 폴더에서 폴더 또는 파일의 링크를 생성</li><li>사용자 API의 '링크 생성'을 실행</li></ul></td></tr><tr><td>링크 미리보기</td><td>링크 수신 화면에 액세스</td></tr><tr><td>링크 다운로드</td><td>링크 수신 화면에서 폴더 또는 파일을 다운로드</td></tr></tbody></table>



**\[Connect User 작업]**

| 동작       | 설명                                        |
| -------- | ----------------------------------------- |
| 파일 업로드   | Connect 폴더에 파일 업로드                        |
| 업데이트     | Connect 폴더에 파일을 업로드한 후 덮어쓰기               |
| 폴더 생성    | Connect 폴더에서 폴더 만들기                       |
| 이름 변경    | Connect 폴더에서 폴더 또는 파일의 이름 변경              |
| 이동       | Connect 폴더에서 폴더 또는 파일 이동                  |
| 이전 버전 복원 | Connect 폴더의 파일을 이전 버전으로 복원                |
| 휴지통 복구   | 휴지통 "Connect"에서 폴더 또는 파일을 복구              |
| 이동 취소    | 폴더 또는 파일 이동을 취소                           |
| 복사       | Connect 폴더에서 폴더 또는 파일 복사                  |
| 복사 취소    | 폴더 또는 파일 사본 취소                            |
| 삭제       | 휴지통 "Connect"의 폴더 또는 파일 삭제                |
| 휴지통      | Connect 폴더의 폴더 파일을 삭제하고 휴지통 "Connect"로 이동 |
| 이동 취소    | 폴더 또는 파일 이동 취소                            |
| 복사 취소    | 폴더 또는 파일 복사 취소                            |
| 삭제 취소    | 폴더 또는 파일 삭제 취소                            |
| 휴지통 취소   | 폴더 또는 파일의 휴지통 "Connect"로 이동 취소            |
| 온라인편집    | 온라인 편집 화면 표시                              |
| 미리보기     | Connect 폴더의 파일 미리보기                       |
| 파일 다운로드  | Connect 폴더 파일 다운로드                        |



{% hint style="warning" %}
**파일 이용 내역을 필터링하여 표시**
{% endhint %}

파일 작업 화면에서 작업 내역을 기간, 사용자, 파일 이름, 작업 및 표시건수로 필터링하여 볼 수 있습니다.

<figure><img src="../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="85.60003662109375">No.</th><th width="655.2000122070312">설명</th></tr></thead><tbody><tr><td>❶</td><td>사용자의 파일 이용 내역을 표시하는 기간을 '최근 7일', '최근 15일', '최근 1개월', '최근 3개월' 중에서 선택합니다.</td></tr><tr><td>❷</td><td>계약 시작부터 현재까지 사용자의 파일 이용 내역이 표시되는 기간을 지정합니다.<br>지정할 수 있는 기간은 12개월입니다.</td></tr><tr><td>❸</td><td>클릭하여 드롭다운 리스트를 표시하고, 사용자의 조작 이력을 필터링하여 표시하고 싶은 액션에 체크합니다.<br>'전체 선택'의 체크를 해제하면, 모든 체크가 해제됩니다.<br>기본적으로는 '전체 선택'에 체크가 되어 있기 때문에, 모든 동작이 검색 대상이 됩니다.</td></tr><tr><td>❹</td><td><p>클릭하여 드롭다운 리스트를 표시하고, 아래 중 하나의 검색 대상을 선택합니다.<br>기본적으로는 '전체'가 선택되어 있기 때문에, 모든 항목이 검색 대상이 됩니다.</p><ul><li>사용자명</li><li>사용자 ID</li><li>파일·폴더명</li><li>폴더 경로</li><li>상세 정보</li></ul><p></p><p><strong>NOTE</strong>:</p><ul><li>검색 대상을 선택하더라도, ❺의 키워드를 입력하지 않는 경우에는 모든 항목이 검색 대상이 됩니다.</li><li><strong>'폴더 경로' 검색은, 계약 플랜이 '프리미엄' 이상인 경우에 이용할 수 있습니다.</strong></li><li>'상세 정보'에서는, 동작이 '이름 변경', '이동', '복사'인 경우에, '파일/폴더명' 열에 표시되는 아래 정보로 검색할 수 있습니다.<br>이름 변경: 변경 전 파일명<br>이동: 이동 원본 폴더 경로<br>복사: 복사 원본 폴더 경로</li></ul></td></tr><tr><td>❺</td><td>❹에서 선택한 검색 대상의 키워드를 입력합니다.<br>부분 일치로 검색되므로, 입력한 키워드가 포함된 검색 대상이 검색 결과에 표시됩니다.<br>예를 들어, '/Shared Box/테스트 폴더 제1계층/테스트 폴더 제2계층/'이라는 폴더 경로가 있는 경우, '/Shared Box/테스트 폴더 제1계층/'을 입력하여 검색하면, 검색 결과에는 아래 폴더 경로가 표시됩니다.<br><em>/Shared Box/테스트 폴더 제1계층/</em><br><em>/Shared Box/테스트 폴더 제1계층/테스트 폴더 제2계층/</em></td></tr><tr><td>❻</td><td>사용자의 파일 이용 내역을 표시하는 건수를 '10', '25', '50', '100' 중에서 선택합니다.</td></tr></tbody></table>



{% hint style="warning" %}
**파일 이용 내역을 CSV 파일로 다운로드 하기**
{% endhint %}

1. 파일 이용 내역에서 'CSV 다운로드' 버튼을 클릭합니다.\
   파일 이용 내역은 대량의 데이터가 될 가능성이 있으므로, 미리 필터링 후다운로드하는 것을 추천합니다.\
   CSV 파일이 다운로드됩니다.

<figure><img src="../../.gitbook/assets/image (1497).png" alt=""><figcaption></figcaption></figure>

&#x20;    &#x20;

2. CSV 파일을 열고 문제없이 표시되는지 확인합니다.

<figure><img src="../../.gitbook/assets/image (1499).png" alt=""><figcaption></figcaption></figure>

&#x20;     CSV 파일의 회사 열은 로그인한 사용자의 유형에 따라 다음과 같이 표시됩니다.

<table><thead><tr><th width="192.79998779296875">사용자 유형</th><th width="553.5999755859375">설명</th></tr></thead><tbody><tr><td>사내 사용자</td><td>사용자가 속한 회사 정보가 표시됩니다.<br>표시 형식: 회사명(회사 ID)</td></tr><tr><td>Guest</td><td>Guest를 초대한 사용자가 속한 회사 정보가 표시됩니다.<br>표시 형식: 회사명(회사 ID)</td></tr><tr><td>Connect User</td><td>Connect User 초대된 측의 회사 정보가 표시됩니다.<br>표시 형식: 회사명</td></tr></tbody></table>
