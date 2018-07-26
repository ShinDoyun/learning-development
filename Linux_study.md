# Linux Shell 요약
### Directory와 파일
#### 커맨드 명령어
- ls -al : 현재 파일 및 디렉토리의 전체 내용을 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_ls_al.PNG)
- pwd : 현재 머물고 있는 디렉토리를 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_pwd.PNG)
- mkdir "" : 현재 머물고 있는 디렉토리에 ""이름의 디렉토리를 생성함<br>
- ls : 현재 디렉토리의 파일들을 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_mkdir.PNG)
- ls -l : 현재 디렉토리의 파일과 디렉토리들을 자세히 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blo1b/master/directory_ls_l.PNG)
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
