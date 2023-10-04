# git-playground1
git 다양한 기능 연습하기

## git amend 마지막에 사용한 커밋에 추가하기

- 소스트리 기준
- 커밋할 때 '마지막 커밋 정정'을 클릭
- 커밋하게 되면, 기존 커밋이 정정되고 새로운 커밋이 추가되지 않는다.

- 원격 저장소의 마지막 커밋을 수정할 때
- 로컬 저장소에서 amend를 사용해 '마지막 커밋 정정' 후 push를 하게 되면 오류메시지 발생

- 푸쉬 사용 시 강제 푸쉬에 체크하고 푸쉬하면 깔끔하게 원격저장소의 커밋도 정정된다.

- 'git commit --amend'
- 커밋 수정 후 덮어쓰기

# Cherry pick
- 필요한 커밋만 딱 가져와서 현재 브랜치에 붙이는 기능
- 현재 브랜치에서 다른 변경사항을 제외한 (예를 들면 버그 수정 등 중요한 커밋) 필요한 커밋만 선택해서 (소스트리 기준 우클릭 - 체리 픽)

- 'git cheery-pick [커밋해시]'
- 커밋이 여러개일 경우
- 'git cheery-pick [커밋해시] [커밋해시2]'