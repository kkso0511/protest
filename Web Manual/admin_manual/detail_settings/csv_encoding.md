---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/detail_settings/csv_encoding
---

# 다운로드하는 CSV 파일의 문자 코드를 설정하는 방법

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 관리자 페이지와 Web 브라우저에서 데이터를 CSV 형식 또는 텍스트 형식으로 다운로드 할 때 사용하는 문자 인코딩을 설정하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* 문자 인코딩 설정은, 기본적으로 'UTF-8 BOM'으로 설정되어 있습니다.
* 이 매뉴얼에서 설정한 문자 코드는, DirectCloud의 관리자 페이지 및 PC Agent에서 CSV 파일과 텍스트 파일을 다운로드하는 모든 기능에 일괄 적용됩니다.\
  관리자 페이지와 PC Agent에서 각각 문자 코드를 개별적으로 설정할 수는 없습니다.\
  또한, 다운로드 시에 메뉴 등에서 개별적으로 문자 코드를 선택할 수는 없습니다.\
  다운로드 기능이 있는 메뉴에 대해서는, 이 메뉴얼의 절차 항목을 참고 부탁드립니다.
* DirectCloud에서는, 'UTF-8'로 내보내는 CSV 파일의 문자 코드로 'BOM 포함'의 'UTF-8'을 채택하고 있습니다.\
  BOM 포함의 경우, 데이터의 처음 몇 바이트가 BOM(Byte Order Mark)이라는 정보를 위해 사용됩니다.\
  Unicode에는 'UTF-8' 외에도 여러 종류가 있지만, 애플리케이션에 따라 이러한 종류를 판별하기 위해 BOM을 사용하는 경우가 있습니다.\
  예를 들어, Microsoft Excel에서는 BOM이 포함되지 않은 파일의 문자 코드를 판별하지 못해, 글자가 깨지는 경우가 발생할 수 있습니다.
*   이 매뉴얼의 절차에 따라 문자 코드를 설정하여 다운로드한 후, 텍스트 편집기로 파일을 열면, 설정한 문자 코드가 아닌 다른 문자 코드로 표시되는 경우가 있습니다.\
    이는 텍스트 편집기가 파일의 문자 정보를 바탕으로 문자 코드를 판단하기 때문에 발생하는 현상입니다.\
    특히 한국어나 일본어처럼 영어가 아닌 문자가 혼재되어 있고 텍스트 정보가 적은 경우에 이 문제가 발생할 수 있습니다.

    문자 깨짐이 발생한 경우에는, 텍스트 편집기의 문자 코드 변환 기능을 이용하여 이 매뉴얼의 절차에서 설정한 문자 코드로 변환함으로써 문자 깨짐을 회피할 수 있습니다.\
    예를 들어, Windows 기본 메모장의 경우, '다른 이름으로 저장'을 선택하면, '문자 코드'에서 문자 코드를 선택하여 덮어쓰기 저장을 할 수 있습니다.\
    그 외에도 많은 텍스트 편집기나 코드 편집기 등에서 문자 코드를 변환할 수 있습니다.
* 'DirectCloud-CONNECT'를 이용할 수 있는 경우, 관리 페이지에 '공유 설정' > 'Connect 관리' 메뉴가 표시됩니다.
* 'DirectCloud-SHIELD DLP'를 계약하고 있는 경우, '공유 설정' > 'DLP 관리' 메뉴가 표시됩니다.
* 'Warm Storage'를 계약하고 있는 경우, '공유 설정' > 'Warm Storage 관리' 메뉴가 표시됩니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**문자 인코딩 선택**
{% endhint %}

1. '공유 설정' > '세부 기능 설정' 메뉴를 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2015).png" alt=""><figcaption></figcaption></figure>



2. 화면을 아래로 스크롤하고 내보낼 때 문자 인코딩 설정에서 인코딩의 다음 문자 코드 중 하나를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2016).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="192">문자코드</th><th>설명</th></tr></thead><tbody><tr><td>UTF-8 BOM 포함</td><td>문자 코드가 UTF-8(유니코드)인 CSV 또는 텍스트 파일을 내보내려면 선택합니다.</td></tr><tr><td>EUC-KR</td><td>문자 코드가 EUC-KR의 CSV 또는 텍스트 파일을 내보내려면 선택합니다.</td></tr></tbody></table>



3. 저장 버튼을 클릭합니다.

<figure><img src="../../.gitbook/assets/image (2017).png" alt=""><figcaption></figcaption></figure>



{% hint style="warning" %}
**다운로드 시 적용되는 문자 코드 설정의 범위**
{% endhint %}

**\[관리자 페이지]**

<table><thead><tr><th width="211.39996337890625">메뉴</th><th>탭, 버튼 등</th><th>대상</th></tr></thead><tbody><tr><td>보안 정책 ＞ 접근 제어</td><td>기기 관리 탭</td><td>승인된 기기의 CSV 다운로드</td></tr><tr><td>계정 관리 ＞ 사용자</td><td>그룹 일괄 등록 버튼</td><td>템플릿 다운로드</td></tr><tr><td></td><td>사용자 일괄 처리 버튼</td><td>·사용자 정보 CSV 다운로드<br>·템플릿 다운로드<br>·그룹 코드 다운로드</td></tr><tr><td>계정 관리 ＞ Guest 관리</td><td>Guest 관리 탭의 Guest 일괄 처리 버튼</td><td>·Guest 정보 CSV 다운로드<br>·템플릿 다운로드</td></tr><tr><td>공유 설정 ＞ Shared Box</td><td>접근 권한 일괄 처리 버튼</td><td>·접근 권한 정보 CSV 다운로드<br>·템플릿 다운로드</td></tr><tr><td></td><td>폴더 일괄 등록 버튼</td><td>템플릿 다운로드</td></tr><tr><td>공유 설정 ＞ DLP</td><td>접근 권한 일괄 처리 버튼</td><td>접근 권한 정보 CSV 다운로드<br>템플릿 다운로드</td></tr><tr><td>공유 설정 ＞ Warm Storage</td><td>접근 권한 일괄 처리 버튼</td><td>접근 권한 정보 CSV 다운로드<br>템플릿 다운로드</td></tr><tr><td></td><td>폴더 일괄 등록 버튼</td><td>템플릿 다운로드</td></tr><tr><td>워크플로우 ＞ 기본 설정</td><td>생성된 워크플로우 목록 탭의 워크플로우 일괄 처리 버튼</td><td>접근 권한 정보 CSV 다운로드<br>템플릿 다운로드</td></tr><tr><td>워크플로우 ＞ 신청 목록</td><td>-</td><td>승인 신청 목록 CSV 다운로드</td></tr><tr><td>용량 관리 ＞ 회사 휴지통</td><td>-</td><td>휴지통에 있는 폴더·파일 정보 CSV 다운로드</td></tr><tr><td>용량 관리 ＞ Guest 휴지통</td><td>-</td><td>휴지통에 있는 폴더·파일 정보 CSV 다운로드</td></tr><tr><td>용량 관리 ＞ Connect User 휴지통</td><td>-</td><td>휴지통에 있는 폴더·파일 정보 CSV 다운로드</td></tr><tr><td>랜섬웨어 대책 ＞ 프로그램 차단 이력</td><td>-</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>랜섬웨어 대책 ＞ 차단 프로그램 목록</td><td>-</td><td>CSV 다운로드</td></tr><tr><td>랜섬웨어 대책 ＞ 허가 프로그램 목록</td><td>-</td><td>CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 바이러스 검출 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 로그인 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 파일 이용 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 파일기한 설정 현황</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 링크 현황</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 링크 이력</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 업로드 요청 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 업로드용 이메일 수신 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 파일 첨부 메일발송 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 인증코드 발급내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 전체권한자 권한 변경 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>로그 현황 ＞ 관리자 페이지 변경 내역</td><td>－</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>SHIELD ＞ 기본 설정</td><td>문서 속성 설정 탭의 CSV 업로드버튼</td><td>템플릿 다운로드</td></tr><tr><td></td><td>문서 속성 설정 탭의 CSV 다운로드 버튼</td><td>문서 속성 CSV 다운로드</td></tr><tr><td>SHIELD ＞ 암호화 문서 목록</td><td>-</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>SHIELD ＞ 암호화 문서 변경 로그</td><td>-</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>SHIELD ＞ 반출 문서 이용 내역</td><td>-</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>SHIELD ＞ 반출 문서 삭제</td><td>-</td><td>검색 결과 CSV 다운로드</td></tr><tr><td>DirectCloud AI ＞ 채팅 로그</td><td>폴더 선택</td><td>메시지 다운로드</td></tr></tbody></table>



**\[PC Web 브라우저]**

| 메뉴·폴더 등 | 탭·버튼 등             | 대상             |
| ------- | ------------------ | -------------- |
| 주소록 메뉴  | CSV 업로드 화면의 템플릿 버튼 | 템플릿 다운로드       |
|         | -                  | 개인 주소록 CSV 다운로 |
