---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-14/warm-storage-cold-storage
---

# Warm Storage와 Cold Storage의 차이

### 개요 <a href="#a03" id="a03"></a>

2025년 7월 15일 업데이트에서 장기 보관에 특화된 Storage인 Cold Storage가 추가되었습니다.\
이 매뉴얼에서는 My Box나 Shared Box 등에서 사용 중인 Hot Storage 외에 제공되는 Warm Storage와 Cold Storage의 기능적 차이점에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 계약 요금제에따라 Warm Storage를 이용할 수 있습니다.
* Cold Storage를 계약한 경우 Cold Storage를 이용할 수 있습니다.
* Warm Storage와 Cold Storage의 폴더 속성에서는 용량 제한과 접근 권한 설정 확장만 설정할 수 있습니다.

***

### 설명

{% hint style="warning" %}
**Hot Storage, Warm Storage, Cold Storage의 차이**
{% endhint %}

DirectCloud에서는 다음의 세 가지 종류의 Storage를 제공합니다.\
각 Storage에서 사용할 수 있는 기능 등이 다르므로, 저장할 데이터의 종류, 작업 내용, 운영 목적 등에 맞춰 설계하는 것을 권장합니다.\
각 Storage는 동시에 병행하여 사용할 수 있습니다.

* **Hot Storage**\
  Shared Box 등에서 사용되는 Storage입니다. 자주 교환되는 데이터를 저장하거나 워크플로우, DirectCloud AI   등 다양한 기능을 활용한 데이터 관리에 적합합니다.\
  Shared Box의 파일은 목적에 따라 Warm Storage나 Cold Storage로 자동 이동되도록 설정할 수 있습니다.
* **Warm Storage**\
  Hot Storage에서 Link History, 파일 잠금, 파일 유효기간 등의 일부 기능을 제외한 Storage입니다. Hot Storage보다 저렴하게 이용할 수 있습니다. 예를 들어, 자주 접근하지 않는 폴더 계층의 데이터를 전체적으로 Warm Storage로 이동하여 장기 보관하면 Shared Box의 Storage를 효율적으로 활용할 수 있습니다. Warm Storage로 이동이 가능한 Hot Storage는 Shared Box만 해당됩니다.
* **Cold Storage**\
  Warm Storage에서 더 많은 기능을 제외한 Storage입니다. Warm Storage보다 저렴하게 이용할 수 있지만, 기능 및 데이터 저장·복원에 관한 제약이 있으므로 주의가 필요합니다.\
  Cold Storage로 이동이 가능한 Hot Storage는 Shared Box만 해당되며, 또한 Warm Storage에서 Cold Storage로의 이동도 가능합니다. &#x20;



{% hint style="warning" %}
**Warm Storage 및 Cold Storage의 사양**
{% endhint %}

| 기능                     | warm storage                                                                               | cold storage                                                                                                                      |
| ---------------------- | ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------- |
| 폴더 경로복사                | ○                                                                                          | ○                                                                                                                                 |
| 폴더 생성                  | ○                                                                                          | ○                                                                                                                                 |
| 업로드                    | ○                                                                                          | ○                                                                                                                                 |
| 미리보기                   | ○                                                                                          | ✕                                                                                                                                 |
| 코멘트                    | <p>✕ <br><br>·코멘트 추가는 불가능합니다. ·코멘트 확인은 미리보기가 활성화된 경우에만 가능합니다. ·코멘트 정보는 유지됩니다.</p>          | <p>✕ <br><br>·코멘트 추가 및 확인은 불가능합니다. ·코멘트 정보는 유지됩니다.</p>                                                                            |
| 온라인 편집                 | ✕                                                                                          | ✕                                                                                                                                 |
| 다운로드                   | ○                                                                                          | ✕                                                                                                                                 |
| 복사                     | <p>Shared Box → Warm: × <br>Warm → Shared Box: × <br>Warm → Warm: ×</p>                    | <p>Shared Box → Cold: × <br>Cold → Shared Box: × <br>Cold → Cold: ×</p>                                                           |
| 이동                     | <p>Shared Box → Warm: ○ <br>Warm → Shared Box: ○ <br>Warm → Warm: ○ <br>Cold → Warm: ×</p> | <p>Shared Box → Cold: ○ <br>Cold → Shared Box: × (복원은 가능) <br>Cold → Cold: ○ <br>Warm → Cold: ○</p>                               |
| 자동 이동                  | ◯                                                                                          | ◯                                                                                                                                 |
| ​Shared Box의 고스트 표시    | ​◯                                                                                         | ​✕                                                                                                                                |
| ​되돌리기                  | <p>​◯<br><br>·폴더와 파일을 즉시 되돌릴 수 있습니다.</p>                                                   | ​-                                                                                                                                |
| ​복구                    | ​-                                                                                         | <p>​△<br><br>·요청 후 최대 12시간 이내에 파일만 복원할 수 있습니다.<br>·매월 1TB당 최대 1000개의 파일까지 복원이 가능합니다.<br>·한 번에 복원 요청할 수 있는 파일 수는 최대 300개까지입니다.</p> |
| ​삭제                    | ​◯                                                                                         | <p>​△<br><br>·저장한 때로부터 90일 후</p>                                                                                                  |
| ​이름 변경                 | ​​◯                                                                                        | <p>​​◯<br><br>·접근 권한이 편집자인 경우에는 90일 후</p>                                                                                         |
| 링크 생성                  | <p>✕<br><br>·설정할 수 없습니다.<br>·링크 정보는 삭제됩니다.</p>                                             | <p>✕<br><br>·설정할 수 없습니다.<br>·링크 정보는 삭제됩니다.</p>                                                                                    |
| 첨부 파일 전송               | ✕                                                                                          | ✕                                                                                                                                 |
| 업로드 요청                 | ✕                                                                                          | ✕                                                                                                                                 |
| 즐겨찾기                   | ◯                                                                                          | <p>✕<br><br>·설정할 수 없습니다.<br>·즐겨찾기 정보는 삭제됩니다.</p>                                                                                  |
| 버전 이력                  | <p>△<br><br>·버전 정보 표시 및 미리보기가 가능합니다.<br>·복원은 불가능합니다.<br>·버전 정보는 유지됩니다.</p>                 | <p>△<br><br>·버전 정보 표시가 가능합니다.<br>·미리보기와 복원은 불가능합니다.<br>·버전 정보는 유지됩니다.</p>                                                         |
| 파일 유효기간                | <p>✕<br><br>·설정할 수 없습니다.<br>·파일 유효기간 정보는 삭제됩니다.</p>                                        | <p>✕<br><br>·설정할 수 없습니다.<br>·파일 유효기간 정보는 삭제됩니다.</p>                                                                               |
| 태그                     | <p>✕<br><br>·설정할 수 없습니다.<br>·태그 정보는 유지됩니다.</p>                                             | <p>✕<br><br>·설정할 수 없습니다.<br>·태그 정보는 유지됩니다.</p>                                                                                    |
| 파일 잠금                  | <p>✕<br><br>·설정할 수 없습니다.<br>·잠금 정보는 삭제됩니다.</p>                                             | <p>✕<br><br>·설정할 수 없습니다.<br>·잠금 정보는 삭제됩니다.</p>                                                                                    |
| 파일 사용 이력               | <p>○<br><br>·조회할 수 있습니다.<br>·Warm Storage의 로그가 추가됩니다.</p>                                  | <p>✕<br><br>·조회할 수 없습니다(로그 정보는 유지됩니다).<br>·Cold Storage의 로그가 추가됩니다.</p>                                                           |
| 전체 검색                  | ◯                                                                                          | <p>✕<br><br>·전체 검색 데이터는 삭제됩니다.</p>                                                                                                |
| DirectCloud 드라이브에서의 사용 | <p>○<br><br>·Warm Storage를 이용할 수 있습니다.</p>                                                 | <p>✕<br><br>·Cold Storage는 이용할 수 없습니다.<br>·휴지통에 Cold Storage 탭이 표시됩니다.</p>                                                        |

