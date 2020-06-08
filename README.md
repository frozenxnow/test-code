1. https://git-scm.com 에 접속하여 Git-2.27.0-64-bit를 다운로드하여 설치

2. 설치시 두 번째 대화상자의 선택 옵션에서 Use Git from the Windows Command Orompt를 선택하여 설치할 것. ( > 그래야 Git Bash 사용 가능)

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
    title: ssh key (제목은 상관 없음)
    key: 붙여넣기 (id_rsa.pub은 메모장으로 열기)
    하여 키를 등록

11. git config --global user.name "사용자아이디"
    git config --global user.email "사용자이메일"

12. git Bash에서 해당 프로젝트 디렉토리를 초기화
    git init 

13. 프로젝트 개발코드 입력하고 저장
    README.md 작성

14. git Bash에서 관리목록으로 추가 
    git add 파일명 또는 git add . (. < 모든 파일 추가)

15. git의 상태 보기( 빨간색은 아직 add하지 않은 것, 초록색은 add한 것)
    git status

16. 작업한 내용의 메시지를 기록 
    git commit -m "커밋할 메시지 입력(작업내용)"

17. 원격 저장소 지정
    git remote add origin 해당 레포시토리 주소
    (https://github.com/frozenxnow/test-code.git)

18. 원격 저장소에 업로드
    git ouosh -u origin master

19. 해당하는 아이디나 이메일, 패스워드를 물어볼 경우 입력하면 업로드 성공
