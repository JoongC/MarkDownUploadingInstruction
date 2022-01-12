Going to Do GitHub By myself

git config —global user.name "Your Name"

git config —global user.email you@example.com

(
—global 이 전체에 적용한다는 뜻
하고 나면 .git/config 에 [user] 라고 생김
)


Thus = global 로 config 하고  새 리포 만들기


- 새로운 리포 & 폴더 만들기
  - 새로 만든 리포에 새로 만든 폴더 올릴거임

- 경로 (command+option+c), (cd+command+v)
  - ex)
  
		cd/Users/joongchoi/Desktop/Project/“NEW FOLDER NAME”
		이동하는 이유는 올릴 파일 지정 / 경로 특정 하기 위함

- init 으로 저장소 초기화
  - to let git track the folder and detect changes to let git 관련 설정들이 해당 폴더에 적용
		
        /Users/joongchoi/.git/ (.git 생김)

- 파일을 하나 만들거여 (명령어 : touch)
  - touch 12321.txt
  - git 이 안 붙는건 git 명령어가 아니라 컴퓨터에 하는 명령이기 때문
  

- git status

- touch 한 파일이 status 에 생긴걸 확인하면 it is time to ‘add’
  - git add . = 전체 업로드
	git add 파일명 = 특정 파일만 업로드

- 다시 git status -> changes to be committed 생김

- git commit -m “메시지 내용”    ->   git status  ->  working tree clean
	
    워킹트리에 add한 파일을 commit 했으니 지금은 empty

	하지만 github에는 올라가지 않음 yet

- commit 은 로컬에서만의 변화
  - git 이 관리하고 있는 상태 -> github에 아직 안 올라감

- (확인단계)
  - cd .git         ->        vi -R config       ->       :q(빠져나옴)
	
    cd 는 지정 폴더로 이동하겠다는 뜻
	
    현재 경로는?

- cd ..
  - 현재 경로는?

- repository in GitHub & the folder I created must be linked
  - GitHub 에 있는 repository address 복사

- git remote
  - 해당 폴더에게 원격저장소(리포지토리)를 알려줌
  - git remote add 이름 (보통 origin) 복사한 주소
	-> remote origin

- 폴더로 다시 돌아와

- git branch
  -  master

- git push origin master

- Put username(JoongC) & Token (repo) that is given