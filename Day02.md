# Github 2일차

## clone & pull

1. 원격 저장소 가져오기
    1. git clone : 원격 저장소의 commit 내용을 모두 가져와서 로컬 저장소 생성
                   -> 원격 저장소를 통째로 복제해서 옮김
        1. ``` bash git clone <원격 저장소 주소> ```
        2. git clone을 통해 생성된 로컬 저장소는 git init과 git remote add가 이미 수행되어 있음

    2. git pull : 원격 저장소의 변경 사항을 가져와서 로컬 저장소 업데이트
        1. 로컬 저장소와 원격 저장소의 내용이 일치하면 git pull 해도 변화 X
        2. ``` bash git pull <저장소 이름> <브랜치 이름> ```
    
    3. git clone & git pull
        1. git clone : git init 처럼 처음에 한 번만 실행 (직접 로컬 저장소를 만들지는 않음)
                       Github에서 저장소를 복제해서 내 컴퓨터에 똑같은 복제본을 만듦
        2. git pull : 로컬 저장소와 원격 저장소의 내용 동기화
                      원격 저장소 변경 내용 -> 로컬 저장소에 반영
        
2. 두 개 이상의 로컬 저장소
    1. 규칙
        1. 로컬 저장소 : TIL-home 
        2. 다른 로컬 저장소 : TIL-class 
        3. Github 원격 저장소 : TIL-remote
    2. 사전 세팅
        1. 홈 디렉토리 안에 TIL-home 생성
        2. Github에서 TIL-remote 이름의 원격 저장소 생성
        3. TIL-home 폴더에서 vscode 열기
        4. ``` bash git init  
                    touch day1.md  
                    git add .  
                    git commit -m "day01 home"  
                    git remote add origin https://github.com/yoodoni/TIL-remote.git  
                    git push origin master ```
                    
        