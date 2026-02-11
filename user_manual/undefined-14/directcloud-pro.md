---
hidden: true
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/undefined-14/directcloud-pro
---

# DirectCloud 파일 미리보기 지원 확장자(Pro 에서 사용 예정)

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에서 지원하는 파일 미리보기 기능의 확장자에 대해 설명합니다.

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 파일 미리보기 기능을 사용하려면, [파일을 다운로드하지 않고 미리 볼 수 있도록 설정하는 방법](https://help.directcloud.net/admin_manual/undefined-6/undefined-2)에 따라 파일 미리보기가 활성화되어 있어야 합니다.
* 업로더 권한의 사용자를 제외하면, 다른 모든 사용자는 파일 미리보기 기능을 사용할 수 있습니다.\
  자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/web), [접근 권한의 종류와 DirectCloud 드라이브 에서 가능한 조작](https://help.directcloud.net/user_manual/undefined-5/directcloud)을 참조하십시오.
* **미리보기가 가능한 확장자 종류는 DirectCloud 서비스 유형에 따라 다릅니다.**\
  **DirectCloud Pro/Pro+에서는 기본 지원 확장자에 53개의 확장자가 추가로 제공됩니다.**
  * **기본 DirectCloud 요금제(Basic \~ Enterprise):**\
    문서·이미지 42종 / 미디어 12종
  * **DirectCloud Pro/Pro+:**\
    문서·이미지 95종 / 미디어 12종
* **DirectCloud 드라이브에서는 My Box, Shared Box, DLP 폴더에 저장된 동영상 및 음성 파일은 미리보기할 수 없습니다.**\
  단, 탐색기에서 파일을 더블 클릭하면 다른 애플리케이션으로 파일을 직접 열 수 있습니다.\
  탐색기에서 파일을 열기 위해서는 마스터, 전체권한, 편집자의 접근 권한이 필요합니다.
* **Web 브라우저에서 미리보기가 가능한 동영상 및 오디오 파일의 종류는 사용중인 브라우저의 사양에 따라 다를 수 있습니다.**
* 텍스트 파일 미리보기는 UTF-8 문자 코드를 지원합니다.\
  그 외 문자 코드로 인코딩된 파일은 글자가 깨질 가능성이 있습니다.
* 한국어 문자 코드인 EUC-KR로 인코딩된 파일은 사용자 페이지의 설정에서 언어를 한국어로 변경하면 미리보기할 수 있습니다.
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
* **iOS 전용 이미지 확장자인 heic, heif 파일을 업로드시, JPEG 파일로 변환하여 업로드합니다.**
* 미리보기 화면이 표시되기까지 시간이 오래 걸리는 경우, Web 브라우저의 캐시를 삭제한 후 다시 시도해 주세요.

### 미리보기 지원 확장자 <a href="#a05" id="a05"></a>

{% hint style="info" %}
**문서와 이미지 총 95종의 확장자 미리보기 지원**
{% endhint %}

<table><thead><tr><th width="149.13336181640625" valign="top">파일 유형</th><th valign="top">모든 요금제 기본 지원</th><th valign="top">Pro 요금제 이상 추가 지원</th></tr></thead><tbody><tr><td valign="top">Word(10)</td><td valign="top">doc, docx, odt, rtf</td><td valign="top">docm, dot, dotm, dotx, fodt, ott</td></tr><tr><td valign="top">Spreadsheet(10)</td><td valign="top">csv, ods, xls, xlsx</td><td valign="top">fods, ots, xlsm, xlt, xltm, xltx</td></tr><tr><td valign="top">Presentation(10)</td><td valign="top">ppt, pptx, odpm</td><td valign="top">pot, potx, potm, pps, ppsm, ppsx, pptm</td></tr><tr><td valign="top">한글(2)</td><td valign="top">hwp, hwpx</td><td valign="top"></td></tr><tr><td valign="top">text(7)</td><td valign="top">txt</td><td valign="top">fodg, fodp, odg, odf, otg, otp</td></tr><tr><td valign="top">Markup(4)</td><td valign="top">html</td><td valign="top">htm, xhtm, xhtml</td></tr><tr><td valign="top">Visio(2)</td><td valign="top">vsd, vsdx</td><td valign="top"></td></tr><tr><td valign="top">Email(2)</td><td valign="top">eml, msg</td><td valign="top"></td></tr><tr><td valign="top">PDF(1)</td><td valign="top">PDF</td><td valign="top"></td></tr><tr><td valign="top">CAD(4)</td><td valign="top"><p>dgn, dwg, dxf<br></p><p>※AutoCAD로 생성한 dwg만 지원</p></td><td valign="top"> dwf</td></tr><tr><td valign="top">이미지(39)</td><td valign="top">jpg, jpeg, png, gif, bmp, cal, dcx, dib, eps, jp2, pcd, pct, psd, ras, tga, tif, tiff</td><td valign="top">cals, cur, cut, dcim, ico, img, jpc, ncr, pbm, pcx, pgm, pic, pict, ppm, psb, sct, sgi, tpic, wbmp, wpg, xbm, xwd<br><br>※heic/heif 파일은 업로드시 jpeg로 전환</td></tr><tr><td valign="top">벡터이미지(1)</td><td valign="top">svg</td><td valign="top"></td></tr><tr><td valign="top">의료(3)</td><td valign="top">dcm</td><td valign="top">dicm, dicom</td></tr></tbody></table>

{% hint style="info" %}
**오디오와 동영상 총 12종의 확장자 미리보기 지원**
{% endhint %}

<table><thead><tr><th width="180.20001220703125">파일 유형</th><th>모든 요금제 기본 지원</th></tr></thead><tbody><tr><td>오디오(7)</td><td>mp3, m4a, aac, aif, aiff, ogg, wav</td></tr><tr><td>동영상(5)</td><td>mp4, mov, m4v, mkv, webm</td></tr></tbody></table>
