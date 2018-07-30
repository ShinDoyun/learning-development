# Linux Shell 요약

### Directory와 파일
#### 커맨드 명령어
- ls -al : 현재 파일 및 디렉토리의 전체 내용을 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_ls_al.PNG)
- pwd : 현재 머물고 있는 디렉토리를 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_pwd.PNG)
- mkdir "" : 현재 머물고 있는 디렉토리에 ""이름의 디렉토리를 생성함<br>
- ls : 현재 디렉토리의 파일들을 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_mkdir.PNG)
- ls -l : 현재 디렉토리의 파일과 디렉토리들을 자세히 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_ls_l.PNG)
- cd "" : "" 디렉토리로 이동<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_cd.PNG)
- rm "" : ""파일을 삭제함<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_rm.PNG)
- rm -r "" : "" 파일 또는 디렉토리를 삭제함<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_rm_r.PNG)

### <br>sudo(substitute user do)
#### sudo 란
- 다른 사용자의 보한 권한, 보통 슈퍼유저로서 프로그램을 구동 시킬 수 있도록 하는 프로그램이다.
#### sudo 명령어가 필요한 커맨드 명령어 예시
- rm -rf : 루트 디렉토리에 있는 모든 파일을 삭제함<br>
- apt-get install "" : ""패키지를 설치함

### <br>nano 에디터
#### Nano란?
- CUI환경에서 파일을  할 수 있는 리눅스 에디터이다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/nano.PNG)

### <br>IO Redirection
#### Output
- IO Redirection Output : 화면으로 출력되는 것을 다른 곳으로 돌려서 파일에 저장 시키는 것
- 1> : 표준 출력 되는 것을 Redirection 한다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/Output_1.PNG)
- 2> : 에러 메시지를 Redirection 한다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/Output_2.PNG)
#### Input
- IO Redirection Input : 입력하는 것을 다른 곳으로 돌려서 파일에 저장 시키는 것.
- cat : 사용자가 입력하는 정보를 받고 출력한다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/cat.PNG)
 - cat example.txt : example.txt을 인자로 하여 cat 프로그램에 입력을 넣음(Command Line Arguments)<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/cat_argv.PNG)
 - cat < example.txt : example.txt을 cat 프로그램에 표준 입력으로 넣음(stdin)<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/cat_stdin.PNG)
 - cat > example.txt : cat 프로그램으로 표준 입력을 받아 example.txt에 넣어줌.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/cat_input.PNG)
- head -n1 : 텍스트의 첫번째 줄 까지만 출력을 함.
  - head -n1 example.txt : example.txt를 인자값으로 씀(Command Line Arguments)<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/head_0.PNG)
  - head -n1 < example.txt : example.txt를 표준 입력으로 넣어줌(stdin)<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/head_1.PNG)
 #### Append
 - \>\> : 파일을 덮어쓰지 않고 원래있던 파일의 내용 뒤에 추가한다.
 - << : 여러 입력을 하나로 합쳐서 입력한다.
 
 ### <br>Shell
 #### Shell
 - Shell : 사용자와 커널 사이의 인터페이스를 감싸는 층이다.
 #### Shell Script
 - Shell Script : 셸에서 돌아가도록 작성된 스크립트이다.
 
 ### <br> Directory 구조
 #### / - Root
 - 모든 파일과 디렉토리들은 Root라는 최상위 디렉토리 부터 시작된다.
 #### /bin - User Binaries
 - 사용자가 사용하는 명령들이 위치해 있는 디렉토리이다.
 #### /sbin - System Binaries   
 - root user나 시스템 관리자들이 사용하는 프로그램들이 있는 디렉토리이다.
 #### /etc - Configuration Files
 - 컴퓨터가 동작하는 설정에 대한 여러가지 변경을 할 수 있는 파일이 있는 디렉토리이다.
 #### /var - Variable Files
 - 내용이 고정된 것이 아니라 바뀌고 증가되고 어떻게 바뀔지 알 수 없는 파일들이 있는 디렉토리이다.
 #### /tmp - Temporary Files
 - 임시로 필요한 파일들이 들어있는 디렉토리이다.
 #### /home - Home Directories
 - 사용자의 파일들이 저장되는 디렉토리이다.
 #### /opt - Optional add-on Applications
 - 사용자가 프로그램을 설치할 때 사용하는 디렉토리이다.
 #### /usr - User Programs
- 다중 사용자의 주요 유틸리티와 어플리케이션을 포함하고 있는 디렉토리.

### 파일 찾는법
#### locate
- locate : mlocate(컴퓨터에 저장되어 있는 파일들의 목록 데이터베이스)를 탐색한다.
- locate \*.log : 확장자가 log인 모든 파일들을 찾는다.
#### find
- find : 직접 컴퓨터의 디렉토리들을 탐색한다
- find / -name \*.log : root디렉토리부터 이름에 .log가 들어가 있는 파일들을 찾는다. <br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/Find.PNG?raw=true)
#### whereis
- whereis : $PATH 와 $MANPATH환경 변수의 경로에 있는 실행 파일, 소스, 매뉴얼 파일을 옵션에 맞게 찾는다.
- whereis "" : ""파일을 찾고 경로를 알려준다.

### <br>프로세스와 실행
#### 프로세스 모니터링
- ps
  - ps : 백그라운드를 제외한 실행중인 프로세스의 리스트를 보여준다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/ps.PNG)
  - ps aux : 백그라운드를 포함한 실행중인 프로세스의 리스트를 보여준다.
  - ps aux | grep apache : 아파치라는 문자열을 포함한 프로세스의 리스트를 보여준다.
- top : 실행 중인 프로세스 리스트를 좀더 세부적이고 보기좋게 보여준다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/Top.PNG)
#### 백그라운드 실행
- Ctrl + z : 실행중인 프로그램을 백그라운드로 보낸다. 이 기능을 실행하면 프로그램이 일시 정지가 된다.
- jobs : 백그라운드 작업들의 목록을 보여준다.
#### 항상 실행
- 데몬(daemon) : 언제나 켜져있는 프로그램.
#### 정기적 실행(cron)
- crontab -e : 정기적으로 실행할 일 들을 에디터로 정의한다.
- crontab -l : 정기적으로 실행중인 프로그램을 보여준다.
#### 쉘을 시작할 때 실행
- .bashrc : bash 쉘이 시작될때 실행하고자 하는 프로그램을 넣을 때 편집 하는 파일.

### <br>다중사용자
#### 사용자확인
- id : 자신이 어떤 계정으로 접속해 있는가.
- who : 이 컴퓨터에 어떤 사람이 접속해 있는가.
#### 사용자의 추가
- useradd -m "" : ""라는 유저를 추가하고 홈디렉토리를 같이 만들어준다.
- usermode -a -G sudo "" : 이미 생성되어 있는 ""라는 유저에게 super user 권한을 부여한다. ![ ](https://github.com/ShinDoyun/learning-development/blob/master/id.PNG)

### <br>권한(chmod)
#### 권한 기본
- r : 읽기 권한
- w : 쓰기 권한
- x : 실행 권한
#### 권한 변경
- chmod o-r "" : ""파일에 대한 other의 read권한을 없앤다.(o : other, u : user)
- chmode u+x "" : ""파일에 대한 user의 execute권한을 준다.
#### directory의 권한
- r : directory의 파일들을 열람 할 수 있는 권한
- w : directory안의 파일을 생성, 수정 삭제 할 수 있는 권한
- x : cd기능을 통해 directory에 들어 갈 수 있는 권한
- chmod -R ''+'' "" : "" directory의 안에있는 폴더까지 재귀적으로 권한을 부여또는 박탈한다.
#### chmod 사용법 정리
- 숫자를 통한 권한 부여 : <br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/chmod_htu.PNG)<br>예시) chmod 124 example.txt
- 권한 부여 대상 설정
  - u : user(owner)
  - g : group
  - o : others
  - a : all
- 권한 부여 방식 설정
  - \+ : 권한 부여
  - \- : 권한 박탈
  - \- : 지정 권한으로 변경
