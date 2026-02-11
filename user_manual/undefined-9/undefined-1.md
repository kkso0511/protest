---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-9/undefined-1
---

# 워크플로우 설정을 변경하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud의 워크플로우를 이용하면 사용자가 아래 작업을 수행할 때 결재자의 승인을 받도록 설정할 수 있습니다.

* 파일 다운로드
* 폴더 및 파일의 링크 생성
* 파일첨부 메일발송
* 파일 업로드

워크플로우 신청자로 지정된 사용자가 대상 기능을 사용하기 위해 승인 신청을 하고, 워크플로우 결재자로 지정된 사용자가 이를 승인함으로써 비로소 작업이 가능해지는 구조입니다.\
이 매뉴얼에서는, 사용자 페이지에서 이미 생성된 워크플로우 설정을 변경하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 다른 워크플로우 작성자가 생성한 워크플로우의 설정을 변경하려면,\
  관리 페이지의 ‘워크플로우 설정’에서 ‘결재선 편집’이 ‘결재선 관리담당자 모두에게 허용’로 설정되어 있어야 합니다.
* Guest는 신청자로 추가할 수 있지만, 참조자·대리 결재자·결재자로 추가할 수는 없습니다.
* 대리 결재자 또는 결재자에 그룹이 등록되어 있는 경우,\
  승인 요청이 제출되면 그 그룹에 속한 모든 사용자에게 승인 요청 알림 메일이 발송됩니다.
* ‘자동 결재’를 체크한 경우, 선택한 일수가 경과한 후 0시 0분에 자동으로 결재됩니다.\
  단, 설정한 날의 자정(0시 0분)까지를 하루로 계산합니다.
* 예를 들어, 설정일이 2023년 8월 7일 13시이고 자동 결재를 1일로 설정한 경우,\
  그날 밤 2023년 8월 8일 0시 0분에 자동 승인됩니다.
* 파일을 지정하여 워크플로우를 적용하는 것은 불가능합니다.
*   ‘다운로드’, ‘업로드’ 워크플로우에서 신청자로 설정된 사용자는 DirectCloud Drive에서 다음 작업을 수행할 수 없습니다.

    * 드래그 앤 드롭을 통한 다운로드 및 업로드
    * 직접 편집
    * 이름 변경
    * 폴더 및 파일 이동
    * 폴더 및 파일 복사
    * 폴더 생성
    * 폴더 및 파일 삭제

    다음 작업은 가능합니다.

    * 마우스 오른쪽 버튼 메뉴를 통한 다운로드 및 업로드
    * 미리보기
    * 온라인 편집
    * 링크 생성
    * 버전 관리
    * 파일 잠금
* ‘링크전송’, ‘파일첨부 메일발송’ 워크플로우에서는 신청자에 대한 작업 제한이 없습니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**자신이 만든 워크플로우 설정 변경**
{% endhint %}

1. 'Workflow' > '결재선' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1002).png" alt=""><figcaption></figcaption></figure>



2. 작성자에 자신의 이름이 표시된 워크플로우를 선택하고 상단의 변경 버튼을 클릭합니다.\
   워크플로우 이름을 클릭하거나 워크플로우를 마우스 오른쪽 단추로 클릭하고 변경을 선택하여 워크플로우를 변경할 수 있는 화면을 표시할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1004).png" alt=""><figcaption></figcaption></figure>



3. 워크플로우 설정을 변경하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1005).png" alt=""><figcaption></figcaption></figure>

워크플로우 설정이 변경되고 '저장되었습니다.'가 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1006).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**다른 사용자가 생성한 워크플로우 설정 변경**
{% endhint %}

1. 'Workflow' > '결재선' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1007).png" alt=""><figcaption></figcaption></figure>



2. 작성자에 다른 사용자의 이름이 표시된 워크플로우를 선택하고 상단의 편집 버튼을 클릭합니다.\
   워크플로우 이름을 클릭하거나 워크플로우를 마우스 오른쪽 단추로 클릭하고 변경을 선택하여 워크플로우를 변경할 수 있는 화면을 표시할 수도 있습니다.

<figure><img src="../../.gitbook/assets/image (1008).png" alt=""><figcaption></figcaption></figure>

새 워크플로우 생성 화면이 표시됩니다.\
다른 사용자가 작성자인 경우 상단에 "ㅇㅇ님이 작성한 결재선으로 수정에 주의가 필요합니다."라는 메시지가 표시됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 104406.png" alt="" width="563"><figcaption></figcaption></figure>

관리 페이지에서 다른 사용자가 워크플로우 설정을 변경할 수 없도록 설정한 경우 상단에 "ㅇㅇ님이 작성한 결재선으로 수정/삭제할 수 없습니다."가 표시되고 워크플로우를 변경할 수 없습니다.

<figure><img src="../../.gitbook/assets/image (1010).png" alt=""><figcaption></figcaption></figure>



3. 워크플로우 설정을 변경하고 확인 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 104406.png" alt="" width="563"><figcaption></figcaption></figure>



4. '수정' 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 104643.png" alt="" width="563"><figcaption></figcaption></figure>

워크플로우 설정이 변경되면 ‘저장했습니다.’라고 표시됩니다.\
또한 워크플로우 작성자의 이름이 변경됩니다.

<figure><img src="../../.gitbook/assets/스크린샷 2025-11-06 104848.png" alt=""><figcaption></figcaption></figure>
