# Here's my daily TIL

## [250116] TIL: Let's Being a Personal Github Page Owner
---
### CLI
* 절대 경로: Root 디렉토리부터 목적지점까지 거치는 모든 경로를 전부 작성한 것
* 상대 경로: 현재 작업 중인 디렉토리를 기준으로 계산된 상대적 위치를 작성한 것

---
### Git
* Git: 분산 버전 관리 시스템
* Git의 영역: Working Directory, Staging Area, Repository
* Git의 동작: git과 관련된 명령어이면 무조건 git으로 시작함
+   ```git init```
+   ```git add``` 
-    ```git add .```: 모든 파일
-    ```git add 파일명```: 특정 파일
+   ```git commit -m "커밋 메시지"``` 

---
---

## [250117] TIL: Create My Portpolio Using Github
---
## Revert&Reset
* Revert 
```git revert <commit id>```
특정 commit을 실행 취소하는 것
취소한 history가 기록되기 때문에 무결성을 보장하며 협업의 신뢰성을 ㄴㅍ임

* Reset
```git reset [옵션] <commit id>```
특정 commit으로 되돌아가는 것
돌아간 지점 다음에 만들어진 commit을 어떻게 처리할 지에 대해 3가지 옵션이 있음
   ```git reset --soft <commit id>``` : commit기록을 staging area에 남김
   ```git reset --mixed <commit id>``` : commit기록을 working directory에 남김
   ```git reset --hard <commit id>```: commit기록을 아예 삭제
   

