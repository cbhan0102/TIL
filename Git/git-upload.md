로컬 프로젝트를 git hub에 올리기

        Git Hub와 Git Bash를 이용해 로컬 프로젝트를 Git Hub에 올리는 방법을 포스팅한다.
        Git Hub에서 레포지토리를 생성했다는 가정 하에 실행

1.생성한 레포지토리의 주소를 복사해둔다.

2.깃허브에 업로드할 프로젝트를 우클릭 - Git Bash Here 선택
업로드 실패해서 파일이 다른 곳으로 이동되거나 손상을 대비해 백업 파일 생성을 추천한다.

3.다음 명령어들을 실행한다.
한꺼번에 복붙할 것이 아니라 직접 한줄한줄 치면서 오류가 나지 않나 확인하며 실행하는 것이 좋다.

        git init //로컬 저장소 생성
        git status // 올라갈 파일 있는지 현재 폴더의 파일들 확인
        
        //둘 중 하나 선택
        git add . // 로컬 저장소에 전체 파일 업로드
        git add [파일명/폴더명] // 로컬 저장소에 특정 파일/폴더 업로드
        
        git commit -m "[푸쉬메세지]" // push시 원하는 메시지 등록 및 commit
        git remote add origin [복사해둔 레포지토리 주소]
        git remote -v // 로컬 저장소가 원격 저장소로 연결
        git push origin master // 아까 커밋한 파일들 원격저장소에 업로드


error1 remote add 명령어가 거부된다면 삭제 후 다시 add하면 된다.
에러명: remote origin already exists.

        git remote rm origin

error2 push 명령어가 거부된다면 강제로 push 시키는 방법도 있다.

        git push -f origin master

정상적으로 작동했다면 레포지토리에 파일들이 추가된
파일이 업로드 되었다고는 뜨는데 레포지토리에서 보이지 않는 경우가 있을 수 있다.
위와 같은 경우에는 브랜치를 확인하고, 다른 브랜치에 업로드 되었으면 해당 브랜치를 default로 변경해주면 된다.

브랜치를 변경하는 방법은 다음과 같다.
       
         Settings - Branches - Default branch


