# gitStudy
git스터디를 위한 프로젝트

1. commit
 - 커밋: git commit -m 'first commit'
 - 마지막 커밋 문구 수정: git commit --amend

2. reset / revert
 - unstage된 파일들 다 리셋: git reset --hard
 - stage -> unstage: git reset [fileName]
 - 이전 커밋으로 돌아가기
   + 커밋들을 취소하기: git reset [--mixed] [commit]
   + 특정 커밋을 취소하는 커밋을 날라기: git revert [commit] / git revert [commit]..[commit]

3. branch / checkout
 - 브랜치 만들고 switch: git checkout -b feature/bugfix_1
 - 브랜치 switch: git checkout master
 - 브랜치 삭제: git branch -d feature/bugfix_1
 

* 옵션들
 - hard: 이전 내용들을 다 지움
 - soft: 이전 내용들을 index에 남김
 - mixed: 모든 옵션의 default 값. 이전 내용을 unstage에 남김
