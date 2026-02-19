---
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/FRc8hBWqHCHYh3E0AhFb/admin_manual/dcmigrator/error_log
---

# DCMigrator 실행 로그 및 오류 로그를 확인하는 방법

### 개요 <a href="#a03" id="a03"></a>

DirectCloud에서는 사내 파일 서버나 네트워크 하드디스크(NAS)에서 DirectCloud로 데이터를 이관하기 위해, 데이터 이관 도구인 DCMigrator(이하, 본 어플리케이션)를 제공합니다.\
DCMigrator에서는 Windows PowerShell을 사용하여, 파일 및 폴더를 DirectCloud로 업로드합니다.\
이 매뉴얼에서는, DCMigrator의 로그를 확인하는 방법에 대해 설명합니다.

***

### 제한·보충사항 <a href="#a04" id="a04"></a>

* DCMigrator를 다운로드 하는 방법은 [DCMigrator 애플리케이션을 다운로드 하는 방법](https://help.directcloud.net/admin_manual/dcmigrator/app_download)을 참조하십시오.

***

### 절차 <a href="#a05" id="a05"></a>

{% hint style="warning" %}
**DCMigrator에 저장된 로그 유형**
{% endhint %}

DCMigrator에 의한 업로드가 완료되면, 실행한 'DCMigrator.exe'가 있는 폴더에 'logs' 폴더가 생성됩니다.\
'logs' 폴더에 저장되는 로그 파일에는 아래의 2종류가 있습니다.

* **정보 로그**\
  DCMigrator를 실행할 때마다, '<20자리 타임스탬프>.log' 형식의 파일명으로 로그 파일이 생성되며, 업로드 실행 결과 메시지가 기록됩니다.\
  기록되는 내용은 DCMigrator 명령 실행 결과로 표시되는 INFO 정보와 동일합니다.
* **에러 로그**\
  실행 결과에 오류가 발생한 경우, '<20자리 타임스탬프>.err' 형식의 파일명으로 로그 파일이 생성되며, 오류 메시지가 기록됩니다.\
  오류의 종류에 따라서는 로그 파일이 생성되지 않고, DCMigrator 명령 실행 결과로만 표시되는 경우도 있습니다.



{% hint style="warning" %}
**정보 로그**
{% endhint %}

| 메시지                                                                                             | 설명                                                                          |
| ----------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| Code:{company\_code}                                                                            | 입력된 회사 ID                                                                   |
| Connected to the DirectCloud.                                                                   | DirectCloud에 성공적으로 로그인                                                      |
| Could not found '{path}' folder in DirectCloud                                                  | 대상 폴더를 찾을 수 없음                                                              |
| <p>DCMigrator is already running.<br>DCMigrator can only run one instance at the same time.</p> | DCMigrator가 이미 시작된 상태에서 DCMigrator를 다시 시작하려고했습니다.                           |
| DCMigrator.exe {version}                                                                        | 실행한 DCMigrator 버전                                                           |
| Deleted {path}                                                                                  | DCMigrator에 "--mirror" 옵션을 사용하여 실행할 때 삭제 된 파일                               |
| Dest:{path}                                                                                     | 마이그레이션 대상 폴더 경로                                                             |
| Device:{device\_id}                                                                             | DCMigrator를 실행한 기기의 기기 ID                                                   |
| Duration                                                                                        | 이관에 소요되는 시간                                                                 |
| Ended:{date} ({time})                                                                           | DCMigrator로 업로드 종료                                                          |
| Failed:{size} {num\_folder} {num\_files}                                                        | 업로드에 실패한 폴더 및 파일의 총 개수                                                      |
| FindFolder ({num\_files} files) {path}                                                          | 대상에 이름, 생성 날짜 및 업데이트 날짜와 시간이 같은 폴더가 있으므로 처리 건너 뛰기                           |
| NewFile {size} {path}                                                                           | 원본 파일을 새로 업로드                                                               |
| NewFolder ({num\_files} files) {path}                                                           | 원본 폴더를 새로 업로드                                                               |
| Opts:{arguments}                                                                                | DCMigrator 명령을 실행할 때 입력한 매개변수                                               |
| Outdated {path}                                                                                 | <p>마이그레이션 대상에 파일 이름 · 작성 일시 · 갱신 일시가 같은 파일이 존재하기 때문에 처리를 건너<br>뜁니다. .</p>   |
| Outdated：{size} {num\_folder} {num\_files}                                                      | 처리가 건너뛰어진 폴더 및 파일의 총 개수                                                     |
| Preparing to connect to the DirectCloud                                                         | 연결 준비 중                                                                     |
| Preparing for migration                                                                         | 이관 준비 중                                                                     |
| Proxy:{proxies}                                                                                 | 프록시 정보                                                                      |
| Ready for migration                                                                             | 이관 준비 완료                                                                    |
| Setting                                                                                         | --settings 옵션으로 불러온 업로드 속도 제한 JSON 파일의 경로 및 파일명                             |
| Source:{path}                                                                                   | 마이그레이션 소스의 폴더 경로                                                            |
| Started:{date\_time}                                                                            | DCMigrator 명령을 실행한 날짜 및 시간                                                  |
| Start migration                                                                                 | 이관 시작                                                                       |
| Total:{size}, {count} Folders, {count} Files                                                    | 업로드된 파일의 총 용량 및 폴더 파일 수                                                     |
| Updated {size} {path}                                                                           | 마이그레이션 대상에 업데이트 날짜와 시간이 다르지만 파일 이름과 작성 날짜와 시간이 같은 파일이 있으므로 원본 파일로 덮어 쓰기 업로드 |
| 사용자 키보드 인터럽트 DCMigrator exit.                                                                   | <p>키보드 입력으로 실행 중인 DCMigrator 중지<br> </p>                                    |
| User:{user\_id}                                                                                 | 입력된 사용자 ID                                                                  |



{% hint style="warning" %}
**에러 로그**
{% endhint %}

여기에서는 에러 로그에 기록된 에러 메시지와 DCMigrator 명령 실행 결과로 표시되는 에러 메시지를 요약합니다.

| 메시지                                                                                                     | 설명                                                       |
| ------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| {path} 'is unsupported path.                                                                            | 대상 폴더 경로에 "내 상자" "공유" 이외의 폴더가 설정되어 있습니다.                 |
| api\_call, {api}, endpoint error 30 count over.                                                         | 동일한 API를 요청할 때 오류가 30회를 초과함                              |
| api\_call, {api}, TypeError, response = {result}                                                        | API를 요청할 때 오류가 발생했습니다.                                   |
| api\_call, Maximum 3 retries failed.                                                                    | API 재시도 처리 가능한 횟수의 상한을 초과했습니다.                           |
| AttributeError: 'NoneType' object has no attribute 'get'                                                | 대상 폴더에 대한 액세스 권한 없음                                      |
| convert error, iso8601\_to\_timestamp={date\_and\_time}                                                 | 시간 형식을 변환하는 중에 오류가 발생했습니다.                               |
| convert error, timestamp\_to\_isoformat={date\_and\_time}                                               | 시간 형식을 변환하는 중에 오류가 발생했습니다.                               |
| Could not found '{path}'                                                                                | 원본 원본 폴더 경로를 찾을 수 없습니다.                                  |
| ctime format exception. {path}, {ctime}                                                                 | 파일 작성 날짜 및 시간을 가져오지 못했습니다.                               |
| <p>DCMigrator can't run more than 5 clients at the same time.<br>Please try again in a few minutes.</p> | 5대 이상의 PC에서 DCMigrator가 병렬로 실행됨                          |
| Deleted Dir Error except. {path} {error\_code}                                                          | 폴더 삭제에 실패했을 때의 에러 코드                                     |
| Deleted Dir Error. {path} {server\_error\_msg}                                                          | 서버 오류로 인해 폴더 삭제에 실패했습니다.                                 |
| 삭제된 파일 오류 except. {path} {error\_code}                                                                  | 파일 삭제에 실패했을 때의 에러 코드                                     |
| 삭제된 파일 오류. {path} {server\_error\_msg}                                                                  | 서버 오류로 인해 파일 삭제에 실패했습니다.                                 |
| ERROR Performing scheduled maintenance.                                                                 | DirectCloud 업데이트 작업 중 DCMigrator 실행                      |
| Failed to login. ({server\_error\_message})                                                             | 서버 오류로 인해 로그인에 실패했습니다.                                   |
| Failed to login. except.                                                                                | 액세스 토큰 확인에 실패했습니다.                                       |
| Failed to login. keyerror.                                                                              | 액세스 토큰이 유효하지 않음                                          |
| Failed to login. result empty                                                                           | 서버로부터 응답이 없고 로그인에 실패했습니다.                                |
| Failed to load settings.json file.                                                                      | 지정한 JSON 파일을 불러오는 데 실패했습니다.                              |
| 파일 정보 오류. {path}                                                                                        | 파일 정보를 얻지 못했습니다.                                         |
| filename Encode except. {path}                                                                          | 파일 경로 및 파일 이름 인코딩에 실패했습니다.                               |
| find\_files except.                                                                                     | DCMigrator를 실행하는 동안 원본 파일을 찾을 수 없습니다.                    |
| get max upload size fail.                                                                               | 업로드 가능한 파일당 용량 한도를 초과했습니다.                               |
| Invalid arguments.                                                                                      | 잘못된 매개변수가 설정됨                                            |
| Invalid JSON format in settings.json file.                                                              | settings.json 파일의 JSON 형식이 올바르지 않습니다.                    |
| json.decoder.JSONDecodeError                                                                            | JSONDecode 관련 에러                                         |
| Local file not found error. {path}                                                                      | 탐색기 폴더 경로의 최대 문자 수를 초과하는 등의 이유로 PC에 저장된 파일에 액세스하지 못했습니다. |
| login token result = empty                                                                              | 서버로부터 응답이 없고 액세스 토큰을 얻지 못했습니다.                           |
| mtime format exception. {path}, {mtime}                                                                 | 파일 업데이트 날짜 및 시간을 가져오지 못했습니다.                             |
| New Folder except. {node} {path}                                                                        | 폴더 업로드에 실패한 경우 대상 폴더 경로                                  |
| New Folder fail. {node} {path} {server\_error\_msg}                                                     | 서버 오류로 인해 폴더 업로드에 실패했습니다.                                |
| PermissionError: \[Errno 13] Permission denied                                                          | 원본 파일에 대한 액세스 권한 없음                                      |
| Please check your arguments.                                                                            | 매개변수를 확인해야 함                                             |
| proxy\_for\_url. fail.                                                                                  | 프록시 설정 실패                                                |
| settings.json must be a JSON object                                                                     | settings.json이 JSON 오브젝트가 아닙니다.                          |
| src dir not found. {path}                                                                               | DCMigrator를 실행하는 동안 원본 파일 경로를 찾을 수 없습니다.                 |
| The max worker only accepts values ​​between 1 and 30.                                                  | 스레드 수의 상한을 초과했습니다.                                       |
| The maximum file size has been exceeded. {path} ({size} > {max\_size})                                  | 폴더 속성의 "용량 제한"에 설정된 폴더 용량의 상한을 초과했습니다.                   |
| The session has expired. Please log in again.                                                           | 세션이 만료되었으므로 다시 로그인해야 합니다.                                |
| The upload timeout only accepts values ​​between 10 and 60 sec.                                         | 업로드 시간 초과 시간 한도를 초과했습니다.                                 |
| tree\_traverse except. node={node}, dirname={dirname},srcpath={dirpath}                                 | 대상 폴더 경로에 대한 정보를 얻지 못한 경우에 대한 자세한 정보                     |
| tree\_traverse fail. {path}                                                                             | 대상 폴더 경로에 대한 정보를 얻지 못했습니다.                               |
| Unknown langcode. ({arg})                                                                               | 명령에 알 수 없는 언어가 입력됨                                       |
| upload fail. {path}({size}) {server\_error\_msg}                                                        | 서버 오류로 인해 파일 업로드에 실패했습니다.                                |
| upload result, except. {result}                                                                         | 시간 초과 이외의 이유로 DCMigrator 실행 결과를 얻지 못했습니다.                |
| upload result, timed out. {date\_time}                                                                  | 처리 시간 초과로 인해 DCMigrator 실행 결과를 얻지 못했습니다.                 |
| upload, Maximum 3 retries failed.                                                                       | 업로드를 재시도할 수 있는 횟수 한도를 초과했습니다.                            |
| upload, result error. request={api}                                                                     | API 오류로 인해 파일 업로드에 실패했습니다.                               |
| upload\_client\_key. Empty                                                                              | 업로드 클라이언트 키를 가져오지 못했습니다.                                 |
| upload\_worker, except.                                                                                 | 업로드 다시 시도에 실패했습니다.                                       |
| upload\_worker, Maximum 5 retries failed.                                                               | 업로드 가능한 횟수 한도를 초과했습니다.                                   |
| upload\_worker, Thread Create except.                                                                   | 사용중인 PC의 리소스 부족 등으로 인해 스레드를 만들지 못했습니다.                   |
