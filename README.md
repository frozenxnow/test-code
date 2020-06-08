1. https://git-scm.com 에 접속하여 Git-2.27.0-64-bit를 다운로드하여 설치

2. 설치시 두 번째 대화상자의 선택 옵션에서 Use Git from the Windows Command Orompt를 선택하여 설치할 것. > 그래야 Git Bash 사용 가능

3. 설치가 끝나면 git bash를 시작메뉴에서 찾아 실행

4. 기본 버전 명령 : git --version, 도움말 확인 명령 : git --help

5. github.com에 접속하여 로그인

6. git bash에서 프로젝트 폴더 생성
    ex1) cd d:\; 
    ex2) mkdir pjw (pwj라는 directory 생성)
    ex3) cd pjw
    ex4) mkdir test-code 
    ex5) ls -al 

7. git bash에서 ssh-keygen 명령으로 암호키 생성

8. 내컴퓨터에서 생성된 키젠이 있는 디렉토리로 이동해서 id_rsa.pub 파일을 찾아 열고 그 안의 내용을 복사하기 한다. (우클릭으로 복사해야함)

9. 로그인 된 github에서 가장 오른쪽 메뉴의 setting> SSH and GPG 선택

10. SSH keys 항목의 [new SSH key]버튼을 눌러 나오는 창에
     title: ssh key(제목은 상관 없음)
     key: 붙여넣기 (id_rsa.pub은 메모장으로 열기)
     하여 키를 등록

11. git config --global user.name "사용자아이디"
    git config --global user.email "사용자이메일"


12. git Bash에서 해당 프로젝트 디렉토리를 초기화
git init 