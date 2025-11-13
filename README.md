# EJEJejje-AH_01_1-Group

* 이 저장소는 1조 프로젝트 저장소입니다
# 메인 브런치 푸쉬는 1명이상의 동의가 필요합니다. 테스트 완료후 푸쉬해주세요!
# test 브런치는 작동단계를 확인하는 곳 입니다. 확인후 PR올려주세요.
# fix 브런치는 코드 수정 후 업로드를 하는 곳 입니다.
# save 브런치는 프로젝트 기간동안 중간저장 파일을 올리는 곳 입니다.


SSH 키 생성 및 GitHub 등록 (처음 한 번만)
SSH 키 생성
ssh-keygen -t ed25519 -C "본인_GitHub_이메일@example.com"
계속 Enter만 눌러도 됨

공개키 복사 (macOS):
pbcopy < ~/.ssh/id_ed25519.pub

Windows(Git Bash):
cat ~/.ssh/id_ed25519.pub
# 출력된 내용 전체 복사


GitHub 웹사이트에서:
오른쪽 위 프로필 → Settings
SSH and GPG keys → New SSH key
Title: 적당히 (예: MyLaptop)
Key: 방금 복사한 내용 붙여넣기 → Add SSH key

연결 테스트:
ssh -T git@github.com

"successfully authenticated" 문구 나오면 성공.
