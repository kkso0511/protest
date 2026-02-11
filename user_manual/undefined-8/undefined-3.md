---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-8/undefined-3
---

# 사용자 페이지에서 파일의 사용 이력을 확인하는 방법

### 개요

이 매뉴얼에서는 사용자 페이지에서 DirectCloud에 저장된 파일의 사용 이력을 확인하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼에서는 Shared Box의 조작 방법을 설명하고 있지만, My Box, Shared Box, Connect, DLP, Warm Storage에서도 동일한 절차로 조작할 수 있습니다.
* Cold Storage에서는 파일 사용 이력을 확인할 수 없습니다.
* 파일을 Cold Storage에서 Shared Box로 복원하면, Cold Storage에서 수행된 작업을 파일 사용 이력에서 확인할 수 있습니다.
* <마스터>, <전체권한>의 접근 권한이 부여된 사용자는 파일 사용 이력을 확인할 수 있습니다.
* Guest는 파일 사용 이력을 확인할 수 없습니다.
* ‘파일 사용 이력’ 화면에는 최근 6개월간의 파일 사용 이력이 최대 50건까지 표시됩니다.
* 파일 사용 이력은 날짜 기준 내림차순으로 표시되며, 정렬 순서를 변경할 수는 없습니다.
* 다음 작업은 파일에 대한 접근 대상이 아니므로, 파일 사용 이력에는 기록되지 않습니다.
  * 폴더에 대한 작업
  * 문서 속성에 관한 작업
  * ‘복사 취소’
  * ‘링크 미리보기’
  * ‘링크 다운로드’
  * ‘복구 요청’
* DirectCloud의 옵션인 ‘DirectCloud-CONNECT’를 이용할 수 있는 경우, 사용자 페이지에 ‘Connect’ 메뉴가 표시됩니다.
* DirectCloud-SHIELD DLP를 계약하고 있는 경우, 사용자 페이지에 ‘DLP’ 메뉴가 표시됩니다.
* Warm Storage를 이용할 수 있는 경우, 사용자 페이지에 ‘Warm Storage’ 메뉴가 표시됩니다.
* Cold Storage를 계약하고 있는 경우, 사용자 페이지에 ‘Cold Storage’ 메뉴가 표시됩니다.

***

### 절차

{% hint style="warning" %}
**파일 사용 이력을 확인하려면**
{% endhint %}

1. 파일 사용 이력을 확인하고자 하는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-05 155950.png" alt=""><figcaption></figcaption></figure>



2. 다음 중 한 가지 방법으로 파일 사용 이력을 표시합니다.

❶ 파일에 체크한 뒤, 상단에 있는 ‘파일 사용 이력’ 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-05 161115.png" alt=""><figcaption></figcaption></figure>

❷ 파일을 마우스 오른쪽 버튼으로 클릭하고 표시된 메뉴에서 ‘파일 사용 이력’을 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-05 161428.png" alt=""><figcaption></figcaption></figure>

❸ 파일 오른쪽에 있는 ▼ 버튼을 클릭하고, 표시된 메뉴에서 ‘파일 사용 이력’을 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-05 161531 (1).png" alt=""><figcaption></figcaption></figure>

‘파일 사용 이력’ 화면에 해당 파일의 접근 이력이 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-05 161929.png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="77">No</th><th width="158.20001220703125">항목</th><th>설명</th></tr></thead><tbody><tr><td>❶</td><td>파일명</td><td>현재 표시 중인 파일 사용 이력의 대상 파일명이 표시됩니다.</td></tr><tr><td>❷</td><td>파일 사용 이력</td><td>동작: 사용 이력에 기록된 작업 내용이 표시됩니다.<br><br>사용자: <br>· 파일을 조작한 사용자 이름이 표시됩니다.<br>· Guest와 Connect User에는 사용자 이름 앞에 ● 배지가 표시됩니다.<br>· 자동 이동이나 자동 삭제로 생성된 기록은 ‘SYSTEM’으로 표시됩니다.<br>· 사용자 이름 위에 커서를 올리면 툴팁으로 사용자 ID를 확인할 수 있습니다.<br>· ‘작업’이 ‘업로드’이고, 업로드 전용 이메일 주소나 링크, 업로드 요청을 통해 업로드된 경우에는 이메일 주소가 표시됩니다.<br>왼쪽에 표시된 ‘i’ 아이콘 위에 커서를 올리면, 이메일 주소 정보를 확인할 수 있습니다.<br><br>날짜/시간: 해당 작업이 수행된 날짜와 시간이 표시됩니다.</td></tr></tbody></table>



{% hint style="warning" %}
**파일 사용 이력의 대상이 되는 작업**
{% endhint %}

사용자가 파일에 대해 아래의 작업을 수행하면, 파일의 사용 이력에 기록됩니다.\
이러한 작업은 관리자 페이지의 '로그 현황'>'파일 이용 내역' 메뉴에도 기록됩니다.

| 항목                     | 설명                                                                                                                                                                                                                                                                                                                                                                            |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 업로드                    | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage 폴더에 파일을 업로드한 경우<br>· 사용자 API의 「파일 업로드」를 실행한 경우</p>                                                                                                                                                                                                                                                    |
| 덮어쓰기 저장                | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage 폴더에 파일을 업로드한 뒤, 동일한 이름으로 덮어쓰기 저장한 경우<br>· 파일 내용을 수정한 후 온라인 편집 화면을 종료한 경우</p>                                                                                                                                                                                                                                        |
| 이름 변경                  | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage 폴더에서 폴더나 파일의 이름을 변경한 경우<br>· 사용자 API의 「폴더 이름 변경」, 「파일 이름 변경」을 실행한 경우<br><br><strong>NOTE</strong><br>오른쪽에 표시된 ‘i’ 아이콘 위에 커서를 올리면, 툴팁으로 변경 전의 이름을 확인할 수 있습니다.</p>                                                                                                                                      |
| 이동                     | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage 폴더에서 폴더 또는 파일을 이동한 경우<br>· Shared Box의 고스트 항목에서 「이동으로 복원」을 실행한 경우<br>· Cold Storage 내에서 폴더 또는 파일을 이동한 경우<br>· 사용자 API의 「폴더 이동」, 「파일 이동」을 실행한 경우<br></p><p><strong>NOTE</strong><br>오른쪽에 표시된 ‘i’ 아이콘 위에 커서를 올리면, 툴팁으로 이동 전 폴더 경로를 확인할 수 있습니다.</p>                                                                    |
| 자동 이동                  | <p>· 폴더 속성 기능을 통해 설정된 Shared Box에서 Warm Storage 또는 Cold Storage로 파일의 자동 이동이 실행된 경우<br></p><p><strong>NOTE</strong><br>오른쪽에 표시된 ‘i’ 아이콘 위에 커서를 올리면, 툴팁으로 이동 전 폴더 경로를 확인할 수 있습니다.</p>                                                                                                                                                                                           |
| 이동 취소                  | 폴더 또는 파일의 이동을 취소한 경우                                                                                                                                                                                                                                                                                                                                                          |
| 복사                     | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더에서 폴더 또는 파일을 복사한 경우<br>· Shared Box의 고스트 항목에서 「복사로 복원」을 실행한 경우<br></p><p><strong>NOTE</strong><br>오른쪽에 표시된 ‘i’ 아이콘 위에 커서를 올리면, 툴팁으로 복사 전 폴더 경로를 확인할 수 있습니다.</p>                                                                                                                                                                    |
| Cold Storage에서 복원      | Cold Storage에서 Shared Box로 파일을 복원한 경우                                                                                                                                                                                                                                                                                                                                         |
| 이전 버전으로 복원             | My Box, Shared Box, Connect 폴더, DLP 폴더의 파일을 이전 버전으로 복원한 경우                                                                                                                                                                                                                                                                                                                    |
| 휴지통                    | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage 폴더, Cold Storage 폴더에서 폴더 또는 파일을 삭제(휴지통으로 이동)한 경우<br>· Connect 폴더의 폴더·파일을 삭제하여 휴지통 「Connect」로 이동한 경우<br>· DLP 폴더의 폴더·파일을 삭제하여 휴지통 「DLP」로 이동한 경우<br>· Warm Storage 폴더의 폴더·파일을 삭제하여 휴지통 「Warm Storage」로 이동한 경우<br>· Cold Storage 폴더의 폴더·파일을 삭제하여 휴지통 「Cold Storage」로 이동한 경우<br>· 사용자 API의 「폴더 삭제」, 「파일 삭제」를 실행한 경우</p> |
| 휴지통 취소                 | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더에서 폴더 또는 파일 삭제(휴지통 이동)를 취소한 경우<br></p><p><strong>NOTE</strong><br>Warm Storage 및 Cold Storage에서는 휴지통으로의 이동을 취소할 수 없습니다.</p>                                                                                                                                                                                                        |
| 휴지통에서 복원               | 휴지통 「My Box / Shared Box」「문서 관리」「Connect」「DLP」「Warm Storage」「Cold Storage」에서 폴더 또는 파일을 복원한 경우                                                                                                                                                                                                                                                                                 |
| 삭제                     | 사용자 휴지통이 「사용하지 않음」으로 설정된 상태에서, My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage, Cold Storage에서 폴더 또는 파일을 삭제한 경우                                                                                                                                                                                                                                                          |
| 삭제 취소                  | <p>사용자 휴지통이 「사용하지 않음」으로 설정된 상태에서, My Box, Shared Box, Connect 폴더, DLP 폴더에서 폴더 또는 파일 삭제를 취소한 경우<br></p><p><br><strong>NOTE</strong><br>Warm Storage 및 Cold Storage 폴더에서는 삭제를 취소할 수 없습니다.</p>                                                                                                                                                                                   |
| 자동 삭제(파일 만료 설정)        | 파일 만료 기능으로 설정된 My Box, Shared Box, Connect 폴더, DLP 폴더의 파일을 자동으로 삭제한 경우                                                                                                                                                                                                                                                                                                        |
| 자동 삭제(폴더 속성 설정)        | 폴더 속성 기능으로 설정된 Shared Box, Connect 폴더, DLP 폴더의 폴더 또는 파일을 자동으로 삭제한 경우                                                                                                                                                                                                                                                                                                          |
| My Box 파일 자동 삭제        | My Box에 설정된 파일 자동 삭제가 실행된 경우                                                                                                                                                                                                                                                                                                                                                  |
| 온라인 편집                 | 온라인 편집 화면을 표시한 경우                                                                                                                                                                                                                                                                                                                                                             |
| 미리보기                   | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage 폴더에서 파일을 미리보기 한 경우<br>· 사용자 API의 「파일 뷰어 생성」을 실행한 경우</p>                                                                                                                                                                                                                                                             |
| DirectCloud Drive에서 열기 | <p>DirectCloud Drive에서 파일을 직접 열람한 경우<br>Windows 탐색기에서 DirectCloud Drive의 파일 표시 방식을 변경한 경우 (썸네일 크기, 미리보기 표시 등)</p>                                                                                                                                                                                                                                                             |
| 오프라인 저장                | My Box 또는 Shared Box 폴더의 파일을 DirectCloud Drive의 오프라인 폴더에 저장한 경우                                                                                                                                                                                                                                                                                                               |
| 다운로드                   | <p>· My Box, Shared Box, Connect 폴더, DLP 폴더, Warm Storage 폴더에서 파일을 다운로드한 경우<br>· 사용자 API의 「파일 다운로드」를 실행한 경우</p>                                                                                                                                                                                                                                                               |
| 첨부파일 전송                | 첨부파일 전송 기능으로 파일을 전송한 경우                                                                                                                                                                                                                                                                                                                                                       |
| 다른 모바일 메일 앱으로 전송       | 모바일 애플리케이션에서 「메일로 전송」을 선택한 경우                                                                                                                                                                                                                                                                                                                                                 |
| 다른 모바일 앱으로 전송          | 모바일 애플리케이션에서 「다음 방법으로 열기」를 선택한 경우                                                                                                                                                                                                                                                                                                                                             |
| 링크 생성                  | <p>· My Box, Shared Box, DLP 폴더에서 폴더 또는 파일의 링크를 생성한 경우<br>· 사용자 API의 「링크 생성」을 실행한 경우</p>                                                                                                                                                                                                                                                                                      |
