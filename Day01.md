# Git - 분산 버전 관리 프로그램



## 1. Git을 쓰는 이유

- 변경사항과 가장 최근의 파일만 저장 -> 메모리 절약



## 2. CLI

1. 디렉토리 이동 : cd 폴더명 (change directory)
2. 디렉토리 생성 : mkdir 폴더명 (make directory)
3. 파일 생성 : touch 파일명
4. 현재 경로의 파일 내역 확인 : ls (list segments)
   1. ls -a : 숨김 폴더, 파일까지 확인 가능
5. mv
   1. 이름 변경 : mv 대상파일 변경이름
   2. 파일 이동 : mv 대상파일 이동위치
6. 파일 제거 : rm 파일/폴더명
7. 현재 경로 파악 : pwd



## 3. 마크다운 문법 

1. 제목 : 앞에 # 붙이기 (#의 개수에 따라 하위 소제목 사용 가능)
2. 목록 (tab으로 하위 목록 생성 가능)
   1. 앞에 - 붙이기 
   2. 앞에 숫자 붙이기
3. 글자 타입
   1. 기울임 : 앞뒤에 *
   2. 굵게 : 앞뒤에 **
   3. 취소선 : 앞뒤에 ~~
   4. 굵게, 기울여서 : 앞뒤에 ***
4. 코드 삽입
   1. 인라인 코드 : 앞뒤에 ` (영문키로 가능)
   2. 블록 코드 : ```언어 -> 코드 입력
5. 링크 : [표시글자] (링크) 사이 공백 X
6. 이미지 : [대체 텍스트] (이미지 주소 링크) 사이 공백 X
7. 인용 : 앞에 >
8. 표 
   1. | 파이프와 - 하이픈 사용 : 열 내용 앞뒤에 |
   2. command + t 로 표 삽입
   3. tab으로 자동 행 추가 가능
9. 원본 소스 보기 : command + /
10. 구분선 : ---



## 4. Git 기초

1. 초기설정
   1. git config --global user.name "유저명"
   2. git config --global user.email "깃허브 이메일"

2. 설정 확인
   git config --global --list

3. 폴더를 저장소(repository)로 만들기 -> 최초 1회만 실행
   git init

4. 파일 만들기
   touch 파일명.확장자

5. 수정 후 파일 저장
   command + s

6. 무대 위로 올리기 (Staging Area)
   git add 파일명.확장자 / git add .

7. 파일 상태 파악
   git status

8. 파일 변경사항 기록 (Commits)
   git commit -m "커밋 메시지"

9. 변경사항 내역 확인
   git log / git log --oneline



## 5. Github 

1. Visual-Studio-Code 에서 연결
   git remote add origin (github url)

2. 연결 확인
   git remote -v

3. 오타가 난 경우
   git remote rm origin

4. Github에 변경사항 백업하기
   git push origin master

