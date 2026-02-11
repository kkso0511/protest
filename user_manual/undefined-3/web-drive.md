---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-3/web-drive
---

# \[Web, Drive] 파일을 다운로드하지 않고 미리보기하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에 저장된 파일을 다운로드하지 않고 미리 보기하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 이 매뉴얼 에서는 Shared Box에서의 작업 방법을 기준으로 설명하고 있지만, Shared Box 이외의 폴더에서도 동일한 절차로 작업하실 수 있습니다.
* 파일 미리보기 기능을 사용하려면, [파일을 다운로드하지 않고 미리 볼 수 있도록 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/undefined-2)에 따라 파일 미리보기가 활성화되어 있어야 합니다.
* 업로더 권한의 사용자를 제외하면, 다른 모든 사용자는 파일 미리보기 기능을 사용할 수 있습니다.\
  자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/web), [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/directcloud)을 참조하십시오.
* **DirectCloud 드라이브에서는 My Box, Shared Box, DLP 폴더에 저장된 동영상 및 음성 파일은 미리보기할 수 없습니다.**\
  단, 탐색기에서 파일을 더블 클릭하면 다른 애플리케이션으로 파일을 직접 열 수 있습니다.\
  탐색기에서 파일을 열기 위해서는 마스터, 전체권한, 편집자의 접근 권한이 필요합니다.
*   파일 미리보기에 해당하는 확장자는 다음과 같습니다.　　

    <table><thead><tr><th width="185">분류1</th><th width="161.800048828125">분류2</th><th>확장자</th></tr></thead><tbody><tr><td>문서·이미지</td><td>문서</td><td>doc, docx, odt, rtf</td></tr><tr><td>문서·이미지</td><td>스프레드시트</td><td>xls, xlsx, ods</td></tr><tr><td>문서·이미지</td><td>프레젠테이션</td><td>ppt, pptx, odp</td></tr><tr><td>문서·이미지</td><td>한글</td><td>hwp, hwpx</td></tr><tr><td>문서·이미지</td><td>텍스트</td><td>txt, csv, html (Shift-JIS로 저장된 HTML을 미리 보려면 meta 태그에 문자 코드를 지정해야 함)</td></tr><tr><td>문서·이미지</td><td>순서도</td><td>vsd, vsdx</td></tr><tr><td>문서·이미지</td><td>이메일</td><td>eml, msg</td></tr><tr><td>문서·이미지</td><td>전자파일</td><td>PDF</td></tr><tr><td>문서·이미지</td><td>CAD</td><td>dgn, dwg, dxf<br>※AutoCAD 이외의 어플리케이션으로 작성된 dwg 파일은 대상외</td></tr><tr><td>문서·이미지</td><td>이미지</td><td>jpg, jpeg, png, gif, bmp, cal, dcx, dib, emf, jp2, pcd, pct, ras, tga, tif, tiff, wmf, svg, dcm</td></tr><tr><td>문서·이미지</td><td>그래픽</td><td>eps, psd</td></tr><tr><td>동영상·음성</td><td>동영상</td><td>mp4, mov</td></tr><tr><td>동영상·음성</td><td>음성</td><td>mp3, m4a</td></tr></tbody></table>
* 텍스트 파일 미리보기는 UTF-8 문자 코드를 지원합니다.\
  그 외 문자 코드로 인코딩된 파일은 글자가 깨질 가능성이 있습니다.
* 한국어 문자 코드인 EUC-KR로 인코딩된 파일은 사용자 페이지의 설정에서 언어를 한국어로 변경하면 미리보기할 수 있습니다.
*   미리보기 화면에서 표시되는 파일에는, 폴더 URL에 URL 파라미터로 고유한 식별 번호가 추가된 미리보기 URL이 사용됩니다.\
    식별 번호의 자릿수에는 별도의 제한이 없습니다.

    파일이 덮어쓰기 저장되어 버전이 변경되더라도, 미리보기 URL은 변하지 않습니다.\\

    * 미리보기 URL 형식:\
      폴더 URL + URL 파라미터
    * URL 파라미터 형식:\
      ?preview= + 식별 번호
*   2023년 3월 14일 업데이트 이전에 즐겨찾기에 등록해 두었던 미리보기 URL에 접근하면, 새로운 미리보기 URL로 리다이렉트됩니다.

    업데이트 이전 미리보기 URL 형식은 아래와 같습니다.

    * 미리보기 URL 형식:\
      폴더 URL + URL 파라미터
    * URL 파라미터 형식:\
      ?preview= + 파일 업데이트 날짜 + 12자리 식별 번호
* 업데이트 이전의 미리보기 URL을 즐겨찾기에 등록한 상태에서 해당 파일의 버전이 업데이트된 경우, 새로운 미리보기 URL로는 리다이렉트되지 않습니다.\
  해당 URL에 접근하면, 파일이 저장된 폴더 화면이 표시됩니다.
*   파일 미리보기 세션 시간은 아래와 같습니다.

    | 애플리케이션                     | 세션 시간                                          |
    | -------------------------- | ---------------------------------------------- |
    | Web 브라우저, DirectCloud 드라이브 | <p>Microsoft Office 파일: 30일<br>그 외 파일: 20분</p> |
    | 모바일 애플리케이션(iOS, Android)   | 모든 파일: 20분                                     |
* 미리보기 세션이 만료된 경우 세션 만료 화면이 표시됩니다.\
  미리보기를 다시 보시려면 화면을 새로고침해 주세요.
* 열람 및 편집 작업에 대해 비밀번호가 설정된 PDF 파일을 미리보려 할 경우,\
  "페이지 로딩에 실패했습니다 - 비밀번호가 필요합니다." 라고 표시됩니다.\
  단, Microsoft Office 파일은 비밀번호가 설정되어 있어도 미리보기가 가능합니다.
* 서로 다른 페이지 크기가 포함된 PDF 파일은 올바른 순서로 미리보기가 되지 않을 수 있습니다.\
  PDF 페이지 크기를 통일하시거나, 파일을 다운로드하여 열어주세요.
* 미리보기 화면이 표시되기까지 시간이 오래 걸리는 경우, Web 브라우저의 캐시를 삭제한 후 다시 시도해 주세요.
* DirectCloud-CONNECT를 이용할 수 있는 경우, 사용자 페이지에 Connect 메뉴가 표시됩니다.
* DirectCloud-SHIELD DLP를 계약한 경우, 사용자 페이지에 DLP 메뉴가 표시됩니다.
* Warm Storage를 사용할 수 있는경우 사용자 페이지에 Warm Storage 메뉴가, DirectCloud 드라이브에는 Warm Storage 폴더가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 미리보기 화면 열기**
{% endhint %}

1. 미리보기할 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1389).png" alt=""><figcaption></figcaption></figure>



2. 다음 방법 중 하나로 미리보기 화면을 표시합니다.

❶  편집하고자 하는 파일을 체크하고 상단의 '미리보기' 버튼을 클릭

<figure><img src="../../.gitbook/assets/image (1390).png" alt=""><figcaption></figcaption></figure>

❷  미리 보려는 파일을 마우스 오른쪽 버튼으로 클릭하고 "미리보기"를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1391).png" alt=""><figcaption></figcaption></figure>

❸  미리보기하려는 파일의 오른쪽에 있는 ▼ 버튼을 클릭하고 표시된 메뉴에서 "미리보기"를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1392).png" alt=""><figcaption></figcaption></figure>

❹  파일의 온라인 편집 화면에서 오른쪽 상단의 "미리보기"버튼을 클릭하십시오.

<figure><img src="../../.gitbook/assets/image (1393).png" alt=""><figcaption></figcaption></figure>

미리보기 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1394).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**DirectCloud 드라이브에서 미리보기 화면 열기**
{% endhint %}

1. 폴더 목록에서 미리 보려는 파일이 저장된 폴더를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1395).png" alt=""><figcaption></figcaption></figure>



2. 미리 보기를 원하는 파일을 마우스 오른쪽 버튼으로 클릭하고 DirectCloud 드라이브 > 미리 보기를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (1396).png" alt=""><figcaption></figcaption></figure>

미리보기 화면이 표시됩니다.

<figure><img src="../../.gitbook/assets/image (1397).png" alt=""><figcaption></figcaption></figure>
