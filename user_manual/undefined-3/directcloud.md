---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-3/directcloud
---

# DirectCloud 드라이브에서 파일을 직접 편집하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud 드라이브의 파일을 편집하는 방법에는 두 가지가 있습니다.\
하나는 Windows 탐색기 등에서 파일의 확장자와 호환되는 애플리케이션으로 파일을 열어 편집하는 직접 편집 방식이며, 다른 하나는 DirectCloud 드라이브의 전용 애플리케이션을 사용해 파일을 편집하는 온라인 편집 방식입니다.\
이 매뉴얼에서는 직접 편집을 통해 파일을 수정하는 방법을 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* **DirectCloud 드라이브는 가상 파일 시스템(Virtual File System)을 사용하므로 계약 계획에 관계없이 DirectCloud 드라이브의 총 용량은 C 드라이브와 동일한 용량이 됩니다.**
*   DirectCloud 드라이브에서 파일을 덮어쓸 때 temp 폴더에 임시 파일이 만들어집니다. 이때 덮어쓰기할 파일과 동일한 하드 디스크 공간이 필요합니다.

    `C:\Users<사용자명>\AppData\Local\DirectCloud Drive\data<회사ID 시퀀스><사용자 시퀀스>\temp`\
    <>로 둘러싸인 폴더는 다음과 같이 환경에 따라 달라집니다.

    <table><thead><tr><th width="186">폴더</th><th>설명</th></tr></thead><tbody><tr><td>&#x3C;사용자 이름></td><td>Windows 사용자 이름</td></tr><tr><td>&#x3C;회사 ID 시퀀스></td><td>DirectCloud 회사 ID 시퀀스를 MD5에서 일정 길이의 문자열로 해시한 문자열<br>예:<br>820e3ca3-b2b4-ec7d-ec6c-8f74c8da83cd</td></tr><tr><td>&#x3C;사용자 시퀀스></td><td>DirectCloud 사용자 시퀀스를 MD5에서 일정 길이의 문자열로 해시한 문자열<br>예제:<br>b21f7f523-975b-3978-1928-ad9009b11b9d</td></tr></tbody></table>
* DirectCloud 드라이브에서 파일을 직접 열려면 다운로드, 파일을 덮어써 저장하려면 업로드 접근 권한이 필요합니다.\
  따라서 파일을 직접 편집하는 사용자에게는 <전체권한> 또는 <편집자> 접근 권한이 부여되어 있어야 합니다.\
  자세한 내용은 [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/directcloud)을 참조하십시오.
* 관리 페이지에서 워크플로우 기본 설정이 사용으로 설정되어 있는 경우 다운로드 또는 업로드 워크플로우를 생성하면 워크플로우 신청자는 파일을 직접 편집할 수 없게 됩니다.
* 배타 제어가 가능한 Microsoft Office 버전은 다음과 같습니다.
  * Microsoft 365
  * Microsoft Office 2021 이후 버전
* 파일에 대한 접근 권한이 부여되어 있는 경우에도 배타 제어가 적용됩니다.
* 볼륨 시리얼 번호 또는 사용자 ID 중 하나라도 다르면 배타 제어가 적용됩니다.
* DirectCloud의 유료 옵션인 DirectCloud-SHIELD IRM에 의해 보안등급 레이블과 irm 확장자가 추가된 파일은 배타 제어가 적용되지 않습니다.
* 또한 DirectCloud-SHIELD IRM으로 보안등급 레이블과 irm 확장자가 추가된 파일은 이름을 지정하여 저장 기능을 사용할 수 없습니다.
* Microsoft Access 파일 및 텍스트 파일은 배타 제어가 적용되지 않습니다.
* 확장자가 xlsm이 아닌 매크로 파일도 배타 제어가 적용되지 않습니다.
* 배타 제어 메시지에는 현재 Windows에 로그인된 사용자 이름이 표시되며, 이는 DirectCloud에서 제어할 수 없습니다.
* DirectCloud 드라이브에서 Microsoft Office 파일을 직접 편집 중인 사용자 A와 동일한 파일을 읽기 전용으로 열어보고 있는 사용자 B가 있을 때, 사용자 A가 파일 메뉴에서 최근에 사용한 항목을 열면 내부적으로 배타 제어가 해제되어 사용자 B가 해당 파일에 쓰기 작업을 할 수 있게 되는 경우가 있습니다.\
  이는 Office 애플리케이션의 동작에 따른 현상으로, 관리 페이지의 드라이브 문자 할당 설정에서 여러 드라이브를 지정한 상태에서 동일한 파일을 연 적이 있는 경우 Word, Excel, PowerPoint의 최근에 사용한 항목에 동일한 파일을 가리키는 서로 다른 경로가 표시되기 때문에 발생합니다.
* Mac 버전 DirectCloud 드라이브에서는 동일한 파일을 여러 사용자가 열어도 배타 제어가 적용되지 않습니다.
* Windows에서 제조사에서 지원하지 않는 애플리케이션은 DirectCloud 드라이브에서 파일을 직접 열어 사용하는 경우에도 지원 대상에 포함되지 않습니다.
* DirectCloud 드라이브에서 지원하지 않는 항목은 다음과 같습니다.
  * 다른 시스템과 연계하여 사용하는 경우
  * 확장자가 xls 또는 xlsx인 파일의 통합 문서 공유 기능
  * Microsoft Office의 매크로를 포함한 액티브 오브젝트 동작
  * Microsoft Excel의 함수 동작
  * 명령 프롬프트에서의 명령 실행(배치 파일 저장은 가능)
* Adobe Photoshop의 PSD 파일을 직접 편집 후 덮어써 저장하면 새 파일로 DirectCloud에 업로드되기 때문에 버전 기록이 남지 않습니다.
* DirectCloud 드라이브에서 특정 폴더를 열 때 액세스할 수 없습니다 오류가 표시된다면 해당 폴더에 저장된 폴더 및 파일의 수가 너무 많을 가능성이 있습니다.\
  Web 브라우저에서 해당 폴더를 열어 폴더 및 파일 수가 1000개 이하가 되도록 정리하는 것을 권장합니다.\
  데이터 저장과 관련된 사양은 [DirectCloud 공통사양](https://help.directcloud.net/user_manual/undefined-14/directcloud) 을 참조하십시오.
* DirectCloud 드라이브에서 파일 속성을 표시한 뒤 Windows와 동일한 방식으로 읽기 전용 또는 숨김 파일 체크를 해도 파일 속성 정보는 변경되지 않습니다.
* Windows의 UNC 경로에서는 DirectCloud 드라이브 애플리케이션 및 DirectCloud 드라이브의 폴더와 파일을 지정할 수 없습니다.
* Microsoft Excel 2007 이전 버전에서 만든 xls 파일을 Microsoft Excel 2007 이후 버전에서 열면, 해당 시점에 파일을 연 사용자의 이름이 파일 헤더에 기록되며 자동으로 덮어써 저장됩니다.\
  이것은 Microsoft Excel의 동작 사양이며 DirectCloud 드라이브에서 제어할 수 없습니다.\
  헤더에 이름이 기록되는 것을 피하려면 이름을 지정하여 저장을 선택하고 xlsx, xlsm, xlsb 등의 확장자로 변경하여 다른 파일로 저장해주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**파일 편집**
{% endhint %}

1. Windows 탐색기에서 DirectCloud 드라이브에서 편집할 파일을 봅니다.
2. 파일을 선택하고 마우스 오른쪽 버튼을 클릭하고 열기를 선택하거나 파일을 두 번 클릭합니다.\
   확장자를 지원하는 응용 프로그램이 시작되고 파일이 표시됩니다.
3. 파일을 편집하고 저장합니다.



{% hint style="warning" %}
**배타 제어에 대하여**
{% endhint %}

다른 사용자가 파일을 직접 편집 중일 때 파일을 열면 배타 제어에 의해 해당 파일은 읽기 전용으로 표시됩니다.\
Microsoft Office를 사용해 파일을 직접 편집하는 경우 DirectCloud 드라이브에서 파일을 열면 동일한 폴더 안에 \~$로 시작하는 임시 파일이 생성됩니다. 이 임시 파일이 존재할 때 배타 제어가 동작합니다.\
배타 제어 대상이 되는 확장자는 다음과 같습니다.

| 프로그램                 | 확장자             |
| -------------------- | --------------- |
| Microsoft Excel      | xls, xlsx, xlsm |
| Microsoft Word       | doc, docx       |
| Microsoft PowerPoint | ppt, pptx       |

{% hint style="info" %}
**NOTE:**\
편집한 파일을 저장하고 Microsoft Office를 종료하면 \~$로 시작하는 임시 파일은 자동으로 삭제됩니다.\
그러나 아래와 같은 원인으로 \~$로 시작하는 파일이 삭제되지 않고 남는 경우가 있습니다.\
\~$로 시작하는 파일이 남아 있으면 다른 사용자가 파일을 열 때 배타 제어 메시지가 표시되거나, 실제 편집 중인 사용자와 다른 사용자의 이름이 표시되는 등의 문제가 발생할 수 있습니다.

* Microsoft Office가 비정상 종료되었거나 강제로 종료된 경우
* 보안 소프트웨어의 간섭이 있었던 경우
* 네트워크 장애가 발생한 경우
* 대상 폴더의 접근 권한 또는 접근 권한 레벨이 변경된 경우
* Microsoft Office 파일을 직접 편집 중에 DirectCloud 드라이브에서 로그아웃했거나 PC를 종료한 경우<br>

이러한 상황에서는 아래 방법 중 하나로 \~$로 시작하는 파일을 삭제해주시기 바랍니다.

* 다른 사용자가 해당 파일을 열고 있지 않은 상태에서 \~$로 시작하는 파일을 삭제
* DirectCloud 드라이브에서 삭제할 수 없는 경우 Web 브라우저 또는 관리 페이지에서 삭제
* \~$로 시작하는 파일을 직접 삭제할 수 없는 경우 해당 접근 권한 또는 접근 권한 레벨을 가진 사용자에게 삭제 요청
{% endhint %}
