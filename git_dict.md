## Git
: Git은 차이점만 저장하는 것이 아니라, 전체 코드를 저장한다. 때문에, 누적되는 추가 계산이 없어 빠르고 가볍다. 

## Process
* add: 변경 사항을 선택하는 과정
* commit: 선택한 변경사항을 하나로 묶어 버전으로 만든 것  
[Git으로 관리하는 4가지 상태]
0) 파일 상태
1) 프로젝트 폴더/작업 공간
2) 프로젝트 폴더/작업공간/로컬저장소(.git 폴더)/스테이지(add로 추가된 파일들)
3) 프로젝트 폴더/작업공간/로컬저장소(.git 폴더)/커밋(commit으로 묶여진 add 파일들) *여기까진 아직 로컬 깃에만 수정된 파일들이 반영되어 있음
4) 원격 저장소 (로컬의 커밋을 그대로 받아옴.)

## Git이 커밋을 관리하는 방식
: 커밋은 이전 커밋을 가리키며, 줄줄이 쌓여간다. 이 때 동시에 2 사람이 이상이 수정을 하고 이를 올린다면 충돌이 발생한다. 이 때는 Branch를 써서 두개를 따로 이전 커밋에 연결해 문제를 해결한다.  
### master
: 가장 최신의 Commit 버전을 가리키는 포인터로, Git이 제공하는 가장 기본적인 Branch이다. 
### User Branch
: 사용자가 직접 생성할 수 있는 Branch로 이 역시 특정 Commit을 가리키는 포인터의 역할을 한다. 이를 통해 분기를 만들고 버전을 나누어 따로 관리할 수 있다. 
### HEAD
: 브랜치 사이와 과거 Commit 등을 자유로이 넘나들 수 있게 해주는 포인터이다. 

## 브랜치 실습 기본: 만들고, 이동한다.
