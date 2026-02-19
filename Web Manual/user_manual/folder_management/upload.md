---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/folder_management/upload
---

# 폴더를 업로드하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 Web 브라우저나 DirectCloud 드라이브를 사용하여 DirectCloud에 폴더를 업로드하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼의 절차에는 Shared Box에서의 작업 방법을 설명하고 있지만, Shared Box 외의 영역에서도 동일한 절차로 작업할 수 있습니다.
* 폴더를 업로드하는 사용자에게는 <마스터>, <전체권한>의 접근권한이 부여되어야 합니다.\
  자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission), [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/d_permission)을 참조하십시오.
* [워크플로우를 활성화하는 방법](https://help.directcloud.net/user_manual/workflow/create_workflow)에서 '결재선 미지정 사용자'가 '제한함'으로 선택되어 있는 경우, 워크플로우의 신청자로 설정된 사용자 외에는 폴더 및 파일을 업로드할 수 없습니다.
* 워크플로우의 업로드는 파일을 대상으로 하기 때문에, [워크플로우를 활성화하는 방법](https://help.directcloud.net/user_manual/workflow/create_workflow)에서 워크플로우의 기본 설정이 사용하기에 체크되어 있으며, '결재선 미지정 사용자'가 '제한함'으로설정되어 있는 경우에는 폴더를 선택하여 업로드할 수 없습니다.
* [업로드 가능한 파일의 크기를 제한하는 방법](https://help.directcloud.net/admin_manual/upload/limit_file_size)에서 업로드 파일의 크기 제한이 활성화되어 있는 경우, 업로드하려는 폴더에 포함된 개별 파일의 용량은 설정된 값으로 제한됩니다.
* [폴더의 용량 제한을 설정하는 방법](https://help.directcloud.net/admin_manual/folder/folder_capacity_limit)에서 폴더에 저장할 수 있는 파일의 총 용량이 제한되어 있는 경우, 업로드 시 폴더에 포함된 파일 용량의 총합이 제한 용량을 초과하면 할당 용량을 초과했기 때문에 파일을 추가할 수 없습니다라는 오류 메시지가 표시되며, 초과 이후의 파일은 업로드되지 않습니다.
* 업로드하려는 폴더 이름에 구자체 문자가 포함되어 있는 경우 일부 문자는 자동으로 신자체로 변환될 수 있습니다.
* 업로드 대상 폴더에 업로드하려는 폴더와 동일한 이름의 폴더가 있는 경우에는 아래와 같이 처리됩니다.
  * 업로드한 폴더가 비어 있는 경우:\
    "동일한 폴더명이 존재합니다." 가 표시되며 폴더는 갱신되지 않습니다.
  * 업로드한 폴더에 다른 이름의 파일이 저장되어 있는 경우:\
    업로드한 폴더에 저장된 파일이 업로드되고, 폴더의 갱신 시각이 업데이트됩니다.
  * 업로드한 폴더에 동일한 이름의 파일이 저장되어 있는 경우:\
    [같은 이름의 파일 업로드 시 처리 기준 설정 방법](https://help.directcloud.net/admin_manual/upload/same_name_file)에 따라 파일이 업로드되며, 폴더의 갱신 시각이 업데이트됩니다.
* 폴더 업로드 시 파일이 덮어쓰기로 저장된 경우에는 파일 버전이 업데이트됩니다.
* 다음 방법으로는 폴더를 업로드할 수 없습니다.
  * Shared Box 링크의 업로드 기능을 이용한 업로드
  * 업로드 요청으로의 업로드
  * 업로드 전용 이메일을 통한 업로드
* Web 브라우저에서 업로드한 폴더에 비어 있는 하위 폴더가 포함되어 있는 경우, 비어 있는 하위 폴더는 업로드되지 않습니다.
* 폴더 트리의 폴더로 폴더 또는 파일을 드래그 앤 드롭하여 업로드하는 경우, 동일한 이름의 파일이 이미 존재하면 관리자 페이지의 '보안 정책'> '반입정책'의 동일 파일명 업로드 설정과 관계없이, 반드시 동일 파일명 업로드 화면에서 처리 방법을 선택해야 합니다.
* 드래그 앤 드롭으로 업로드한 뒤 폴더 또는 파일이 표시된 상태에서 멈추는 경우에는 화면을 새로 고침해 주십시오.
* DirectCloud-SHIELD IRM이 활성화된 폴더에 기밀 문서 판정 기준에 해당하는 파일이 포함된 폴더를 업로드하는 경우, 업로드된 파일에는 자동으로 기밀도 라벨과 irm 확장자가 추가됩니다.
*   DirectCloud 드라이브에서 업로드가 완료되기 전에 네트워크 연결이 끊어진 경우에는 아래 절차로 업로드 작업을 다시 시작하십시오.

    1. 작업 트레이에서 DirectCloud 드라이브 아이콘을 클릭
    2. 상태 탭을 클릭
    3. '업로드 대기 중인 파일이 〇개 있습니다.'에 표시된 재시도 아이콘을 클릭



***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서의 폴더 업로드**
{% endhint %}

1. 폴더를 업로드할 폴더를 표시합니다.

<figure><img src="../../.gitbook/assets/image (1270).png" alt=""><figcaption></figcaption></figure>



2. 업로드할 폴더를 드래그 앤 드롭합니다.

<figure><img src="../../.gitbook/assets/image (1271).png" alt=""><figcaption></figcaption></figure>

폴더와 폴더의 파일이 업로드  됩니다.\
업로드한 폴더에 하위 폴더가 포함되어 있으면 모든 폴더와 파일이 업로드됩니다.

<figure><img src="../../.gitbook/assets/image (1272).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 폴더 업로드**
{% endhint %}

1. 폴더를 업로드할 폴더를 표시합니다.

<figure><img src="../../.gitbook/assets/image (1273).png" alt=""><figcaption></figcaption></figure>



2. 업로드할 폴더를 DirectCloud 폴더로 드래그 앤 드롭합니다.

<figure><img src="../../.gitbook/assets/image (1274).png" alt=""><figcaption></figcaption></figure>

DirectCloud 폴더에 폴더가 복사됩니다.



3. PC에 폴더를 남기지 않고 DirectCloud로 이동하려면 "Shift" 키를 누른 상태에서 PC의 폴더를 DirectCloud로 드래그 앤 드롭합니다.



{% hint style="warning" %}
**업로드 알림 이메일 확인**
{% endhint %}

아래의 조건을 충족한 상태에서 폴더를 업로드하면 "업로더"의 공유자권한이 부여된 사용자 이외에도 "○○ 에 신규파일이 업로드 되었습니다."라는 제목의 알림 메일이 전송됩니다.&#x20;

* 관리자가 폴더 속성의 '메일 알림'을 '사용함'으로 설정했습니다.
* 사용자 페이지에서 알림 메일을 수신할지 여부를 설정할 수 있도록 하는 방법 으로 '통지 메일'이 '수신됨'으로 설정되어 있습니다.

<figure><img src="../../.gitbook/assets/image (1275).png" alt=""><figcaption></figcaption></figure>
