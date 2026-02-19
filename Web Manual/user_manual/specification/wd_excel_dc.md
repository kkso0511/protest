---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/user_manual/specification/wd_excel_dc
---

# \[Web, Drive] DirectCloud가 지원하는 Microsoft Excel의 사용자 정의

### 개요 <a href="#a03" id="a03"></a>

이 매뉴얼에서는 DirectCloud에서 지원하는 Microsoft Excel의 사용자 정의에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* <업로더> 접근 권한이 부여된 사용자를 제외한 사용자는 파일 미리보기 기능을 이용할 수 있습니다.\
  자세한 내용은 [접근 권한의 종류와 Web 브라우저에서 가능한 조작](https://help.directcloud.net/user_manual/access_permission/w_permission)을 참고해 주시기 바랍니다.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**Web 브라우저에서 지원하는 Microsoft Excel의 사용자 정의**
{% endhint %}

1. Web 브라우저에서 지원하는 Microsoft Excel의 사용자 정의는 다음과 같습니다.

* 예: 입력 텍스트가 '2021/12/01'인 경우

| 사용자 정의                          | Microsoft Excel에서의 표시 | Web 브라우저에서의 표시     |
| ------------------------------- | --------------------- | ------------------ |
| \[$-en-US]d-mmm-yy              | 1-Dec-21              | 1-Dec-21           |
| \[$-en-US]d-mmm                 | 1-Dec                 | 1-Dec              |
| \[$-en-US]mmm-yy                | Dec-21                | Dec-21             |
| \[$-en-US]h:mm AM/PM            | 12:00 AM              | 12:00 AM           |
| \[$-en-US]h:mm:ss AM/PM         | 12:00:00 AM           | 12:00:00 AM        |
| \[$-en-US]mmm-yyyy              | Dec-2021              | Dec-2021           |
| \[$-ja-JP]yyyy/m/d(dddd)        | 2021/12/1(水曜日)        | 2021/12/1(水曜日)     |
| 12 月 1 日                        | 12 月 1 日              | 12 月 1 日           |
| h:mm                            | 0:00                  | 0:00               |
| h:mm:ss                         | 0:00:00               | 0:00:00            |
| mm:ss                           | 00:00                 | 00:00              |
| mm:ss.0                         | 00:00.0               | 00:00.0            |
| yyyy"年"m"月"d"日";@               | 2021 年 12 月 1 日       | 2021 年 12 月 1 日    |
| yyyy"年"m"月";@                   | 2021 年 12 月           | 2021 年 12 月        |
| m"月"d"日";@                      | 12 月 1 日              | 12 月 1 日           |
| yyyy/m/d;@                      | 2021/12/1             | 2021/12/1          |
| \[$-en-US]d-mmm;@               | 1-Dec                 | 1-Dec              |
| \[$-en-US]d-mmm-yy;@            | 1-Dec-21              | 1-Dec-21           |
| \[$-en-US]dd-mmm-yy;@           | 01-Dec-21             | 01-Dec-21          |
| \[$-en-US]mmm-yy;@              | Dec-21                | Dec-21             |
| \[$-en-US]mmmm-yy;@             | December-21           | December-21        |
| \[$-en-US]mmmmmm;@              | D                     | D                  |
| \[$-en-US]mmmmmm-yy;@           | D-21                  | D-21               |
| \[$-ja-JP]yyyy/m/d              | 2021/12/1             | 2021/12/1          |
| \[$-ja-JP]yyyy"年"m"月"d"日"       | 2021 年 12 月 1 日       | 2021 年 12 月 1 日    |
| \[$-ja-JP]yyyy"年"m"月"           | 2021 年 12 月           | 2021 年 12 月        |
| \[$-ja-JP]m"月"d"日"              | 12 月 1 日              | 12 月 1 日           |
| \[$-ja-JP]h:mm AM/PM            | 12:00 午前              | 12:00 午前           |
| \[$-ja-JP]h:mm:ss AM/PM         | 12:00:00 午前           | 12:00:00 午前        |
| \[$-ja-JP]h:mm                  | 0:00                  | 0:00               |
| \[$-ja-JP]h:mm:ss               | 0:00:00               | 0:00:00            |
| \[$-ja-JP]h"時"mm"分"             | 0 時 00 分              | 0 時 00 分           |
| \[$-ja-JP]h"時"mm"分"ss"秒"        | 0 時 00 分 00 秒         | 0 時 00 分 00 秒      |
| \[$-ja-JP]yyyy/m/d h:mm         | 2021/12/1 0:00        | 2021/12/1 0:00     |
| \[$-ja-JP]mm:ss.0               | 00:00.0               | 00:00.0            |
| \[$-ja-JP]yyyy"年"m"月"d"日"       | 2021 年 12 月 1 日       | 2021 年 12 月 1 日    |
| \[$-ja-JP]yyyy-mm-dd;@          | 2021-12-01            | 2021-12-01         |
| \[$-ja-JP]yyyy"年"m"月"d"日";@     | 2021 年 12 月 1 日       | 2021 年 12 月 1 日    |
| \[$-ja-JP]yyyy"年"m"月";@         | 2021 年 12 月           | 2021 年 12 月        |
| \[$-ja-JP]m"月"d"日";@            | 12 月 1 日              | 12 月 1 日           |
| yyyy-mm-dd;@                    | 2021-12-01            | 2021-12-01         |
| \[$-en-US]yyyy/m/d h:mm AM/PM;@ | 2021/12/1 12:00 AM    | 2021/12/1 12:00 AM |
| yyyy/m/d h:mm;@                 | 2021/12/1 0:00        | 2021/12/1 0:00     |
| m/d;@                           | 12/1                  | 12/1               |
| m/d/yy;@                        | 12/1/21               | 12/1/21            |
| mm/dd/yy;@                      | 12/01/21              | 12/01/21           |
| \[$-ja-JP]m/d/yy                | 12/1/21               | 12/1/21            |
| \[$-ja-JP]d-mmm-yy              | 1-12-21               | 1-12-21            |
| \[$-ja-JP]d-mmm                 | 1-12                  | 1-12               |
| \[$-ja-JP]mmm-yy                | 12-21                 | 12-21              |
| \[$-ja-JP]mm:ss                 | 00:00                 | 00:00              |
| \[$-ja-JP]yyyy/m/d;@            | 2021/12/1             | 2021/12/1          |
| \[$-ja-JP]yyyy/m/d h:mm AM/PM;@ | 2021/12/1 12:00 午前    | 2021/12/1 12:00 午前 |
| \[$-ja-JP]yyyy/m/d h:mm;@       | 2021/12/1 12:00 午前    | 2021/12/1 12:00 午前 |
| \[$-ja-JP]m/d;@                 | 12/1                  | 12/1               |
| \[$-ja-JP]m/d/yy;@              | 12/1                  | 12/1               |
| \[$-ja-JP]mm/dd/yy;@            | 12/01/21              | 12/01/21           |



2. Web 브라우저에서 지원하지 않는 Microsoft Excel의 사용자 정의는 다음과 같습니다.&#x20;

* 예: 입력 텍스트가 '2021/12/01'인 경우

| 사용자 정의                               | Microsoft Excel에서의 표시 | Web 브라우저에서의 표시     |
| ------------------------------------ | --------------------- | ------------------ |
| h"時"mm"分"                            | 2021/12/1 0:00        | 44531              |
| h"時"mm"分"ss"秒"                       | 0 時 00 分 00 秒         | 44531              |
| yyyy/m/d h:mm                        | 2021/12/1 0:00        | 2021/12/01 0:00    |
| yyyy"年"m"月"d"日"                      | 2021 年 12 月 1 日       | 2021/12/01         |
| yyyy"年"m"月"                          | 2021 年 12 月           | 44531              |
| m"月"d"日"                             | 12 月 1 日              | 44531              |
| \[$-ja-JP]ge.m.d                     | R3.12.1               | 44531              |
| \[$-ja-JP]ggge"年"m"月"d"日"            | 令和 3 年 12 月 1 日       | 44531              |
| yyyy/m/d                             | 2021/12/1             | 2021/12/01         |
| m/d/yy                               | 2021/12/1             | 2021/12/01         |
| \[$-ja-JP-x-gannen]ggge"年"m"月"d"日";@ | 令和 3 年 12 月 1 日       | ggg 年 m 月 d 日      |
| \[$-ja-JP]gge"年"m"月"d"日";@           | 令 3 年 12 月 1 日        | gg 年 m 月 d 日       |
| \[$-ja-JP-x-gannen]gge"年"m"月"d"日";@  | 令 3 年 12 月 1 日        | gg 年 m 月 d 日       |
| \[$-x-sysdate]dddd, mmmm dd, yyyy    | 2021 年 12 月 1 日       | 水曜日, 12 月 01, 2021 |
| yyyy/m/d(aaa)                        | 2021/12/1(水)          | 2021/12/1()        |
| \[$-ja-JP]ge.m.d                     | R3.12.1               | 44531              |
| \[$-ja-JP]ggge"年"m"月"d"日"            | 令和 3 年 12 月 1 日       | 44531              |
| \[$-ja-JP]ggge"年"m"月"d"日";@          | 令和 3 年 12 月 1 日       | ggg 年 m 月 d 日      |
| \[$-ja-JP]gge"年"m"月"d"日";@           | 令 3 年 12 月 1 日        | gg 年 m 月 d 日       |



{% hint style="warning" %}
**DirectCloud 드라이브가 지원하는 Microsoft Excel 사용자 정의**
{% endhint %}

1. DirectCloud 드라이브가 지원하는 Microsoft Excel의 사용자 정의는 다음과 같습니다.

* 예: 입력 텍스트가 '2021/12/01'인 경우

<table><thead><tr><th>사용자 정의</th><th width="241">Microsoft Excel에서의 표시</th><th>DirectCloud 드라이브에서의 표시</th></tr></thead><tbody><tr><td>[$-en-US]d-mmm-yy</td><td>1-Dec-21</td><td>1-Dec-21</td></tr><tr><td>[$-en-US]d-mmm</td><td>1-Dec</td><td>1-Dec</td></tr><tr><td>[$-en-US]mmm-yy</td><td>Dec-21</td><td>Dec-21</td></tr><tr><td>[$-en-US]h:mm AM/PM</td><td>12:00 AM</td><td>12:00 AM</td></tr><tr><td>[$-en-US]h:mm:ss AM/PM</td><td>12:00:00 AM</td><td>12:00:00 AM</td></tr><tr><td>[$-en-US]mmm-yyyy</td><td>Dec-2021</td><td>Dec-2021</td></tr><tr><td>[$-ja-JP]yyyy/m/d(dddd)</td><td>2021/12/1(水曜日)</td><td>2021/12/1(水曜日)</td></tr><tr><td>12 月 1 日</td><td>12 月 1 日</td><td>12 月 1 日</td></tr><tr><td>h:mm</td><td>0:00</td><td>0:00</td></tr><tr><td>h:mm:ss</td><td>0:00:00</td><td>0:00:00</td></tr><tr><td>mm:ss</td><td>00:00</td><td>00:00</td></tr><tr><td>mm:ss.0</td><td>00:00.0</td><td>00:00.0</td></tr><tr><td>yyyy"年"m"月"d"日";@</td><td>2021 年 12 月 1 日</td><td>2021 年 12 月 1 日</td></tr><tr><td>yyyy"年"m"月";@</td><td>2021 年 12 月</td><td>2021 年 12 月</td></tr><tr><td>m"月"d"日";@</td><td>12 月 1 日</td><td>12 月 1 日</td></tr><tr><td>yyyy/m/d;@</td><td>2021/12/1</td><td>2021/12/1</td></tr><tr><td>[$-en-US]d-mmm;@</td><td>1-Dec</td><td>1-Dec</td></tr><tr><td>[$-en-US]d-mmm-yy;@</td><td>1-Dec-21</td><td>1-Dec-21</td></tr><tr><td>[$-en-US]dd-mmm-yy;@</td><td>01-Dec-21</td><td>01-Dec-21</td></tr><tr><td>[$-en-US]mmm-yy;@</td><td>Dec-21</td><td>Dec-21</td></tr><tr><td>[$-en-US]mmmm-yy;@</td><td>December-21</td><td>December-21</td></tr><tr><td>[$-en-US]mmmmmm;@</td><td>D</td><td>D</td></tr><tr><td>[$-en-US]mmmmmm-yy;@</td><td>D-21</td><td>D-21</td></tr><tr><td>[$-ja-JP]yyyy/m/d</td><td>2021/12/1</td><td>2021/12/1</td></tr><tr><td>[$-ja-JP]yyyy"年"m"月"d"日"</td><td>2021 年 12 月 1 日</td><td>2021 年 12 月 1 日</td></tr><tr><td>[$-ja-JP]yyyy"年"m"月"</td><td>2021 年 12 月</td><td>2021 年 12 月</td></tr><tr><td>[$-ja-JP]m"月"d"日"</td><td>12 月 1 日</td><td>12 月 1 日</td></tr><tr><td>[$-ja-JP]h:mm AM/PM</td><td>12:00 午前</td><td>12:00 午前</td></tr><tr><td>[$-ja-JP]h:mm:ss AM/PM</td><td>12:00:00 午前</td><td>12:00:00 午前</td></tr><tr><td>[$-ja-JP]h:mm</td><td>0:00</td><td>0:00</td></tr><tr><td>[$-ja-JP]h:mm:ss</td><td>0:00:00</td><td>0:00:00</td></tr><tr><td>[$-ja-JP]h"時"mm"分"</td><td>0 時 00 分</td><td>0 時 00 分</td></tr><tr><td>[$-ja-JP]h"時"mm"分"ss"秒"</td><td>0 時 00 分 00 秒</td><td>0 時 00 分 00 秒</td></tr><tr><td>[$-ja-JP]yyyy/m/d h:mm</td><td>2021/12/1 0:00</td><td>2021/12/1 0:00</td></tr><tr><td>[$-ja-JP]mm:ss.0</td><td>00:00.0</td><td>00:00.0</td></tr><tr><td>[$-ja-JP]yyyy"年"m"月"d"日"</td><td>2021 年 12 月 1 日</td><td>2021 年 12 月 1 日</td></tr><tr><td>[$-ja-JP]yyyy-mm-dd;@</td><td>2021-12-01</td><td>2021-12-01</td></tr><tr><td>[$-ja-JP]yyyy"年"m"月"d"日";@</td><td>2021 年 12 月 1 日</td><td>2021 年 12 月 1 日</td></tr><tr><td>[$-ja-JP]yyyy"年"m"月";@</td><td>2021 年 12 月</td><td>2021 年 12 月</td></tr><tr><td>[$-ja-JP]m"月"d"日";@</td><td>12 月 1 日</td><td>12 月 1 日</td></tr><tr><td>yyyy-mm-dd;@</td><td>2021-12-01</td><td>2021-12-01</td></tr><tr><td>[$-en-US]yyyy/m/d h:mm AM/PM;@</td><td>2021/12/1 12:00 AM</td><td>2021/12/1 12:00 AM</td></tr><tr><td>yyyy/m/d h:mm;@</td><td>2021/12/1 0:00</td><td>2021/12/1 0:00</td></tr><tr><td>m/d;@</td><td>12/1</td><td>12/1</td></tr><tr><td>m/d/yy;@</td><td>12/1/21</td><td>12/1/21</td></tr><tr><td>mm/dd/yy;@</td><td>12/01/21</td><td>12/01/21</td></tr><tr><td>[$-ja-JP]m/d/yy</td><td>12/1/21</td><td>12/1/21</td></tr><tr><td>[$-ja-JP]d-mmm-yy</td><td>1-12-21</td><td>1-12-21</td></tr><tr><td>[$-ja-JP]d-mmm</td><td>1-12</td><td>1-12</td></tr><tr><td>[$-ja-JP]mmm-yy</td><td>12-21</td><td>12-21</td></tr><tr><td>[$-ja-JP]mm:ss</td><td>00:00</td><td>00:00</td></tr><tr><td>[$-ja-JP]yyyy/m/d;@</td><td>2021/12/1</td><td>2021/12/1</td></tr><tr><td>[$-ja-JP]yyyy/m/d h:mm AM/PM;@</td><td>2021/12/1 12:00 午前</td><td>2021/12/1 12:00 午前</td></tr><tr><td>[$-ja-JP]yyyy/m/d h:mm;@</td><td>2021/12/1 12:00 午前</td><td>2021/12/1 12:00 午前</td></tr><tr><td>[$-ja-JP]m/d;@</td><td>12/1</td><td>12/1</td></tr><tr><td>[$-ja-JP]m/d/yy;@</td><td>12/1</td><td>12/1</td></tr><tr><td>[$-ja-JP]mm/dd/yy;@</td><td>12/01/21</td><td>12/01/21</td></tr></tbody></table>



2. DirectCloud 드라이브가 지원하지 않는 Microsoft Excel의 사용자 정의는 다음과 같습니다.

* 예: 입력 텍스트가 '2021/12/01'인 경우

<table><thead><tr><th>사용자 정의</th><th width="242.5999755859375">Microsoft Excel에서의 표시</th><th>DirectCloud 드라이브에서의 표시</th></tr></thead><tbody><tr><td>h"時"mm"分"</td><td>2021/12/1 0:00</td><td>44531</td></tr><tr><td>h"時"mm"分"ss"秒"</td><td>0 時 00 分 00 秒</td><td>44531</td></tr><tr><td>yyyy/m/d h:mm</td><td>2021/12/1 0:00</td><td>2021/12/01 0:00</td></tr><tr><td>yyyy"年"m"月"d"日"</td><td>2021 年 12 月 1 日</td><td>2021/12/01</td></tr><tr><td>yyyy"年"m"月"</td><td>2021 年 12 月</td><td>44531</td></tr><tr><td>m"月"d"日"</td><td>12 月 1 日</td><td>44531</td></tr><tr><td>[$-ja-JP]ge.m.d</td><td>R3.12.1</td><td>44531</td></tr><tr><td>[$-ja-JP]ggge"年"m"月"d"日"</td><td>令和 3 年 12 月 1 日</td><td>44531</td></tr><tr><td>yyyy/m/d</td><td>2021/12/1</td><td>2021/12/01</td></tr><tr><td>m/d/yy</td><td>2021/12/1</td><td>2021/12/01</td></tr><tr><td>[$-ja-JP-x-gannen]ggge"年"m"月"d"日";@</td><td>令和 3 年 12 月 1 日</td><td>ggg 年 m 月 d 日</td></tr><tr><td>[$-ja-JP]gge"年"m"月"d"日";@</td><td>令 3 年 12 月 1 日</td><td>gg 年 m 月 d 日</td></tr><tr><td>[$-ja-JP-x-gannen]gge"年"m"月"d"日";@</td><td>令 3 年 12 月 1 日</td><td>gg 年 m 月 d 日</td></tr><tr><td>[$-x-sysdate]dddd, mmmm dd, yyyy</td><td>2021 年 12 月 1 日</td><td>水曜日, 12 月 01, 2021</td></tr><tr><td>yyyy/m/d(aaa)</td><td>2021/12/1(水)</td><td>2021/12/1()</td></tr><tr><td>[$-ja-JP]ge.m.d</td><td>R3.12.1</td><td>44531</td></tr><tr><td>[$-ja-JP]ggge"年"m"月"d"日"</td><td>令和 3 年 12 月 1 日</td><td>44531</td></tr><tr><td>[$-ja-JP]ggge"年"m"月"d"日";@</td><td>令和 3 年 12 月 1 日</td><td>ggg 年 m 月 d 日</td></tr><tr><td>[$-ja-JP]gge"年"m"月"d"日";@</td><td>令 3 年 12 月 1 日</td><td>gg 年 m 月 d 日</td></tr></tbody></table>
