# Git (2nd day)

## What I missed (Review)

**git push *origin(원격 저장소) master(브랜치)***  기울임 글씨는 임의 지정된 용어 (변동 가능)

**git remote -v** : origin list 확인

**git remote rm *remote_url*** : 로컬 저장소에 등록된 원격 저장소 삭제

**git branch -v** : branch list 확인

**git log --oneline** : id 너무 길때 간략하게 표시시

## Revert & Reset (권장x)

**git revert <commit_id>** : 단일 commit의 실행 취소 (revert했다는 기록이 남음)

**git reset [옵션] <commit_id>** : 특정 commit으로 돌아갔을 때 그 이후의 commit 전부 삭제 or 삭제된 commit 복원

**git reflog** : 삭제된 commit 기록 확인인

옵션 soft, mixed, hard 에 따라 저장되는 장소가 달라짐

**--soft** : commit을 삭제하고 modification을 staging area에 저장 (초록색 글씨)

**--mixed** : commit을 삭제하고 modification을 working directory에 저장 (빨간간색 글씨)

**--hard** : commit을 삭제하고 modification 완전삭제

## Undoing

**restore** : modify한 내용 전부 삭제 (위험하니까 쓰지 마라)

**stash** : modify한 내용을 숨겨서 다른 곳에 저장 (Recommend)

**git stash** : modify한 내용을 stash

**git stash list** : stash들의 목록 확인 (일련번호 존재)

**git stash pop** : stash했던 변경사항 다시 불러오기기