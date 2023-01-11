원격 저장소 연결 및 끊기 (git remote)

깃 사용시 현재 로컬 저장소 (local repository)에 연결되어있는
원격저장소(remote repository)를 연결을 끊고 다시 연결을 하는 방법을 간단히 포스팅한다.

1.git remote -v 명령어를 사용하여 현재 연결되어있는 원격 레파지토리를 확인해보자.
        $ git remote -v

        github원격 저장소와 연결되어 있는 것을 확인할 수 있다. 해당 원격저장소의 연결을
        제거하기 위해서 git remote remove<name>옵션을 사용해주면 연결되어있는
        저장소를 간단하게 끊을 수 있다.

        -> git remote remove origin
        
        이후 다시 -v 옵션을 통해 확인해보면 연결된 원격 저장소가 없는 것을 확인할 수 있다.

        다시 원격 저장소와 연결하고 싶다면 git remote add <name> <url> 옵션을 사용하면 된다.
        -> git remote add origin http~

        


