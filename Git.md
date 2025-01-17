# Git & Cli

VS code Terminal에서 Git Bash 설정

Github 회원가입 + Repository 만들기

__origin__ : 원격 저장소 

__master__ : working directory

---
## 명령어
__git init__ : master 설정 = commit 작성 시작한다

__git add "file name"__ : 변경사항 stage로 보내기기

__git commit -m "commit name"__ : commit 생성해서 저장

**git remote add origin *remote repo url***  : 원격 저장소 url origin에 저장

**git push origin master** : 원격 저장소에 commit 목록 업로드

**git pull origin master** : 원격 저장소의 변경사항 저장장 (업데이트)

**git clone *remote_repo_url*** : 원격 저장소 전체를 복제 (다운로드)

**.gitignore** : 공개하고 싶지 않은 문서 파일명 저장

---
### 주의사항

- 서로 다른 사람이 같은 파일을 수정하고 업로드 할 경우 나중에 업로드하는 쪽이 에러 발생 = 먼저 업로드 된 수정사항이 반영되지 않은 파일이라 에러


---

## Cli

Linux Vi 찾아볼것

ls : 디렉토리 안의 파일명 표시

mkdir : 새 폴더 만들기

rm : 파일 (폴더 제외) 삭제

cd : 디렉토리 변경

.. : 상위 디렉토리

