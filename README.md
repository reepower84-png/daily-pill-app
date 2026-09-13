# 데일리약 — 체크 페이지

[데일리약](https://github.com/reepower84-png/daily-pill)의 **체크 페이지**입니다.

매일 아침 9시 50분에 디스코드로 "오늘 약 드세요" 알림이 오면, 그 링크로 들어와
큰 체크박스를 한 번 누르면 끝입니다. 아래 달력에 먹은 날과 깜빡한 날이 바로 칠해집니다.

- **먹음** 초록 · **깜빡** 분홍 · **오늘·예정** 빈칸
- 지난 날짜를 눌러 고칠 수 있습니다 (체크를 깜빡한 날도 나중에 채울 수 있게)
- 연속 일수 · 이번 달 복용률 · 깜빡한 날 수

- 주소: <https://reepower84-png.github.io/daily-pill-app/>
- 이 저장소는 공개지만 **비밀은 하나도 없습니다.** 복용 기록은 비공개 저장소
  `daily-pill` 에 있고, 이 페이지는 브라우저에 저장된 개인 토큰으로 그 파일을 고칩니다.
- 토큰은 이 기기의 `localStorage` 에만 있습니다. 서버로 보내지 않습니다.

## 다른 데일리 앱과 다른 점

데일리북·데일리잉글리쉬 앱은 GitHub **Actions 를 실행시키는** 버튼이라 토큰에
`Actions: Read and write` 가 필요했습니다. 이 앱은 워크플로를 거치지 않고
**기록 파일을 직접 고칩니다.** 체크 한 번에 20초를 기다리게 하면 다음부터 안 누르니까요.

그래서 필요한 권한이 다릅니다 — **`Contents: Read and write`** 하나입니다.

## 처음 설정

1. 페이지를 열면 토큰을 물어봅니다.
2. [Fine-grained PAT 발급](https://github.com/settings/personal-access-tokens/new)
   - Repository access: **Only select repositories** → `daily-pill`
   - Permissions: **Contents** = Read and write
3. 붙여넣고 저장하면 끝. 이후로는 링크만 열면 됩니다.
4. (선택) 브라우저 메뉴 → '홈 화면에 추가' 하면 앱처럼 쓸 수 있습니다.
