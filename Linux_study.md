# Linux Shell 요약
### Directory와 파일
#### 커맨드 명령어
- ls -al : 현재 파일 및 디렉토리의 전체 내용을 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_ls_al.PNG?raw=true)
- pwd : 현재 머물고 있는 디렉토리를 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_pwd.PNG?raw=true)
- mkdir "" : 현재 머물고 있는 디렉토리에 ""이름의 디렉토리를 생성함<br>
- ls : 현재 디렉토리의 파일들을 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_mkdir.PNG?raw=true)
- ls -l : 현재 디렉토리의 파일과 디렉토리들을 자세히 보여줌<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_ls_l.PNG?raw=true)
- cd "" : "" 디렉토리로 이동<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_cd.PNG?raw=true)
- rm "" : ""파일을 삭제함<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_rm.PNG?raw=true)
- rm -r "" : "" 파일 또는 디렉토리를 삭제함<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/directory_rm_r.PNG?raw=true)
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
- 1\> : 표준 출력 되는 것을 Redirection 한다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/Output_1.PNG?raw=true)
- 2\> : 에러 메시지를 Redirection 한다.<br>![ ](https://github.com/ShinDoyun/learning-development/blob/master/Output_2.PNG?raw=true)
#### Input
- IO Redirection Input : 입력하는 것을 다른 곳으로 돌려서 파일에 저장 시키는 것.
- cat : 입력 되는 것을 Redirection 한다.
  - cat example.txt : example.txt를 인자값으로 씀(Command Line Arguments)
  - cat < example.txt : example.txt에 표준 입력으로 값을 넣음(stdin)
- head -n1 : 텍스트의 첫번째 줄 까지만 출력을 함.
  - head -n1 example.txt : example.txt를 인자값으로 씀(Command Line Arguments)
  - head -n1 < example.txt : example.txt를 표준 입력으로 넣어줌(stdin)
 #### Append
 - \>\> : 파일을 덮어쓰지 않고 원래있던 파일의 내용 뒤에 추가한다.
 - << : 합쳐서 입력한다.
