# git-learning
--깃허브 한방정리--<br>
주요 프로그램 gitbach, 깃허브데스크탑, 소스트리<br>
gitbach를 채택! https://git-scm.com/ 사이트주소<br>
1.긍정적 설치<br>
2.초기설정<br>
$git config --global user.name "id"   --아이디설정<br>
$git config --global user.mail "mail" --메일설정<br>
3.폴더관련<br>
$pwd 현재위치<br>
$ls == dir 검색<br>
$cd 경로이동 ~처음으로 ./작업중인 디렉토리 ../상위디렉토리<br>
$mkdir 폴더명 폴더만들기<br>
$rm 폴더명, -r 폴더명 하위디렉토리 전부삭제<br>
4.깃 지역저장소 만들기<br>
$git init 깃초기화 현재폴더를 지역저장소로 .git폴더가생김<br>
$git status 깃 상태보기<br>
$git log 커밋내역이나 메세지확인, --oneline 최근것만 확인<br>
$git add 작업트리에서 스테이지에 올린다 * 모든것, .변동된것, 파일명 한개씩가능<br>
$git commit 스테이지에서>>지역저장소로 commit -m "메세지" 메세지 남길수있다<br>
$git commit -am "mesaage" Add와commit과 메세지를 한번에<br>
5.브랜치 만들기<br> 
$git branch 브랜치 상태 확인<br>
$git branch 브랜치명 브랜치를 만든다<br>
$git checkout 브랜치명 브랜치 이동<br>
$git log --oneline --branches 각브랜치의 커밋을 볼수있다<br>
$git log --oneline --branches --graph 브랜치 구조를 볼수있다 ex 같은줄기에서 분기했지만 다른 커밋을 만든구조<br>
6.브랜치 병합하기<br>
$git merge 병합할 브랜치 네임 <br>
$git reset 수정중인 파일 되돌리기 한번은 commit한 시점에서<br>
$git stash 파일 감추기<br>
$git stash pop 최근항목으로 되돌리기<br>
$git stash apply 저장했던 내용은 그대로 남겨두기<br>
7.원격 저장소에 백업하기<br>
$git 원하는 폴더를 만들고 init 깃초기화<br>
$git remote add origin 깃주소 +폴더명 +선택사항<br>
$git remote -v 연동되었는지 확인<br>
$git push -u origin master 원격저장소에 파일올리기 <br>
$git pull origin master 파일 가져오기<br>
$git rm -r --cached 파일명 or * 파일 삭제 <br>
8.팀원일시 플레이<br>
$git clone 깃주소  경로설정을 잘해야한다 깃에있는 파일복사<br>
$git config user.name , $git config user.email 아이디,이메일 설정<br>
$git remote -v 연동되었는지 확인하고<br>
$git fetch 원격저장소정보를 임시저장소로 가져온다<br>
$git checkout FETCH_GEAD 임시저장소로 이동<br>
$git status , git log 확인하고<br>
$git checkout master 이동하고<br>
$git commit -am "메세지" 한번에 하거나 아니면 add와 commit -m "메세지" 두번에 나눠서 하고<br>
$git merge FETCH_GEAD 임시저장소와 병합한다<br>
$git commit 다시 커밋해주고<br>
$git push 원격저장소로 밀어 넣는다<br>
한줄요약<br>
clone >> 작업 >> fetch >> merge >> commit >> push 끝!<br>
고급 스킬<br>
https://gmlwjd9405.github.io/2018/05/25/git-add-cancle.html<br>
