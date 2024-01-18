## Nextjs13을 활용한 간단한 예제

- Router 방식으로는 `App Router` 사용
- 백엔드는 `pocketbase`를 활용하여 데이터 구현

## 백엔드 서버 구동되도록 하는 방법

오픈소스 백엔드인 [`pocketbase`](https://pocketbase.io/)를 활용하여 데이터를 저장하고 불러오는 예제이기 때문에 local 환경에서 테스트하기 위해서는 다음과 같이 서버가 구동되는 환경을 만들어주어야 합니다.

1. pocketbase 서버 구동하기

   vscode 터미널에서

   - `Window` 운영체제인 경우 `pocketbase serve` 입력
   - `Mac`인 경우 `./pocketbase serve` 입력

   하여 백엔드 서버가 구동되는 환경을 만들어줍니다.

   만약 정상적으로 구동되는 상태라면 다음과 같은 메세지가 출력됩니다.

   ```bash
   2024/01/18 13:46:34 Server started at http://127.0.0.1:8090
   ├─ REST API: http://127.0.0.1:8090/api/
   └─ Admin UI: http://127.0.0.1:8090/_/
   ```

2. 위 Admin UI url 주소로 접속하기
   - 위 메세지에 출력된 Admin UI url 주소로 접속
   - 간단한 계정 생성? 단계인 이메일 및 비밀번호 입력 후 로그인하기

---

⚠ pocketbase의 collections 생성과 document 생성, 그리고 데이터 접근 권한 설정 등과 관련한 사용방법은 해당 예제의 중점적으로 소개할 내용이 아니기 때문에 브라우저 검색을 통해 확인 바랍니다.
