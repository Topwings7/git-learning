# git-learning
--깃허브 한방정리
주요 프로그램 gitbach, 깃허브데스크탑, 소스트리
gitbach를 채택! https://git-scm.com/ 사이트주소 
1.긍정적 설치 
2.초기설정
$git config --global user.name "id"   --아이디설정
$git config --global user.mail "mail" --메일설정
3.폴더관련
$pwd 현재위치
$ls == dir 검색
$cd 경로이동 ~처음으로 ./작업중인 디렉토리 ../상위디렉토리
$mkdir 폴더명 폴더만들기
$rm 폴더명, -r 폴더명 하위디렉토리 전부삭제
4.깃 지역저장소 만들기
$git init 깃초기화 현재폴더를 지역저장소로 .git폴더가생김
$git status 깃 상태보기 
$git log 커밋내역이나 메세지확인, --oneline 최근것만 확인
$git add 작업트리에서 스테이지에 올린다 * 모든것, .변동된것, 파일명 한개씩가능
$git commit 스테이지에서>>지역저장소로 commit -m "메세지" 메세지 남길수있다
$git commit -am "mesaage" Add와commit과 메세지를 한번에
5.브랜치 만들기 
$git branch 브랜치 상태 확인
$git branch 브랜치명 브랜치를 만든다
$git checkout 브랜치명 브랜치 이동
$git log --oneline --branches 각브랜치의 커밋을 볼수있다
$git log --oneline --branches --graph 브랜치 구조를 볼수있다 ex 같은줄기에서 분기했지만 다른 커밋을 만든구조
6.브랜치 병합하기
$git merge 병합할 브랜치 네임 
$git reset 수정중인 파일 되돌리기 한번은 commit한 시점에서
$git stash 파일 감추기
$git stash pop 최근항목으로 되돌리기
$git stash apply 저장했던 내용은 그대로 남겨두기
7.원격 저장소에 백업하기
$git 원하는 폴더를 만들고 init 깃초기화
$git remote add origin 깃주소 +폴더명 +선택사항
$git remote -v 연동되었는지 확인
$git push -u origin master 원격저장소에 파일올리기 
$git pull origin master 파일 가져오기
8.팀원일시 플레이
$git clone 깃주소  경로설정을 잘해야한다 깃에있는 파일복사
$git config user.name , $git config user.email 아이디,이메일 설정
$git remote -v 연동되었는지 확인하고
$git fetch 원격저장소정보를 임시저장소로 가져온다
$git checkout FETCH_GEAD 임시저장소로 이동
$git status , git log 확인하고
$git checkout master 이동하고
$git commit -am "메세지" 한번에 하거나 아니면 add와 commit -m "메세지" 두번에 나눠서 하고
$git merge FETCH_GEAD 임시저장소와 병합한다
$git commit 다시 커밋해주고
$git push 원격저장소로 밀어 넣는다
한줄요약
clone >> 작업 >> fetch >> merge >> commit >> push 끝!



