# 25/07/17 소개합니다요 SSAFY 
<br>이건 git 명령어입니다. 
```git
git touch 파일명
```
```git
git mkdir 폴더명
```
```git
git add 파일명
```
```git
git commit -m "커밋내용"
```
```git
git push origin master
```
<br><br>
# git의 커밋 되돌리기 2가지 장법
## revert : 재설정
- 변경사항을 안전하게 실행 취소할 수 있도록 도와주는 순방향 실행 취소 작업
- commit 기록에서 commit을 삭제하거나 분리하는 대신, 지정된 변경 사항을 반전시키는 새 commit생성
- git에서 기록이 손실되는 것을 방지하며 기록의 무결성과 협업의 신뢰성을 높임

git - revert의 명령어 <br>
```
git revert commit ID
```
<br><br>
## rest : 되돌리기
- 시계를 마치 과거로 돌리는 듯한 행위
- 특정 commit으로 되돌아 갔을 때, 되돌아간 commit 이후의 commit은 모두 삭제
git - rest의 3가지 옵션<br>
```
git reset 옵션 commit ID
```
- --soft : 삭제된 commit의 기록을 staging area에 남김
- --mixed : 삭제된 commit의 기록을 working directory에 남김 (기본 옵션 값)
- --hard : 삭제된 commit의 기록을 남기지 않음
<br><br>
## Staging area에 올라간 파일 Unstage 하기

```
git rm --cached
```
```
git restore --staged
```
