### Git 초기 세팅
git --configure 
git --configure

### Git commit 순서
git add filename  
git commit -m 'message'
git push origin master


### 로컬 저장소에 원격 저장소 주소를 알려주는 명령어
git remote add origin GitHubAddress

### 단어 정리
origin : 원격 저장소 의미
master: 기본 커밋을 올리는 줄기

### 교훈
* If I meet the error, when I use the sourcetree, then Open the terminal and solve the problem on it. If I solve it throught the CLI, then sourcetree also represents it too. Cause most of the ways to solve the problem are based on CLI.

### Git Branch & Merge
* 2개 이상의 브런치를 합치는 것을 말한다. 
* Merge의 종류
1. Merge commit
2. Fast-Forward
3. Conflict  
: 서로 다른 브런치의 수정 내용이 같을 경우

#### Conflict 해결 방법
1. Master 브랜치를 땡겨와서 분기 Branch에서 병합  
:  충돌 리스크가 있기에 함께 쓰는 master 브랜치로 병합을 하지 않고, 먼저는 Branch에서 병합을 해본다.
2. 분기 Branch에서 병합한 병합 커밋을 master 브랜치에 반영  
: 병합된 커밋이 없는 것을 확인하고 이를 master branch에 반영함  
\* master branch에 바로 이를 반영해도 되지만, 협업하는 사람들에게 문제를 일으킬 수 있으니 자신의 Branch에서 미리 병합을 해보고 문제가 없을 때 이를 master에 반영하는 것이 좋다.