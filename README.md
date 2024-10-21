# javascript-calculator-precourse

## 기능 요구 사항

### 입출력

**사용자 입력 받기**

- [ ] `Console.readLineAsync()`를 사용하여 사용자에게 입력을 요청
- [ ] 사용자에게 "덧셈할 문자열을 입력해 주세요."라는 메시지를 출력
- [ ] 만약 사용자가 아무것도 입력하지 않으면 `[ERROR] 입력이 없습니다.`라는 메시지를 출력하고 프로그램을 종료

**계산 결과 출력**

- [ ] 계산이 완료된 결과를 `Console.print()`를 사용하여 출력
- [ ] `"결과 : {결과값}"` 형식으로 출력

### 문자열 파싱

**커스텀 구분자 추가**

- [ ] 기존 구분자인 쉼표(`,`)와 콜론(`:`) 외에 커스텀 구분자를 추가할 수 있도록 구현
- [ ] 입력 문자열이 `//`로 시작하고 `\n` 이전에 문자열이 있으면 해당 문자열을 커스텀 구분자로 사용

**구분자 처리**

- [ ] 입력 문자열을 구분자를 기준으로 분리하여 배열로 반환

### 숫자 변환 및 검증

**문자열을 숫자로 변환하기**

- [ ] 분리된 문자열 배열을 순회하면서 숫자로 변환
- [ ] 변환된 값이 숫자가 아닌 경우(`NaN`일 경우), 검증 오류가 발생하도록 처리

**에러 처리**

- [ ] 숫자로 변환된 배열이 비어 있거나 숫자가 아닌 값이 포함된 경우 `[ERROR] 잘못된 입력입니다.`라는 메시지를 출력하고 프로그램을 종료
- [ ] 음수가 포함된 경우 `[ERROR] 음수는 허용되지 않습니다.`라는 메시지를 출력하고 프로그램을 종료

### 테스트

**테스트 실행 및 통과 확인**

- [x] 여러 테스트 케이스를 작성
- [ ] `npm test` 명령어를 사용하여 테스트를 실행

## 프로그래밍 요구 사항

- Node.js 20.17.0 버전에서 실행 가능해야 한다.
- 프로그램 실행의 시작점은 `App.js`의 `run()`이다.
- `package.json` 파일은 변경할 수 없으며, **제공된 라이브러리와 스타일 라이브러리 이외의 외부 라이브러리는 사용하지 않는다.**
- 프로그램 종료 시 `process.exit()`를 호출하지 않는다.
- 프로그래밍 요구 사항에서 달리 명시하지 않는 한 파일, 패키지 등의 이름을 바꾸거나 이동하지 않는다.
- 자바스크립트 코드 컨벤션을 지키면서 프로그래밍한다.
  - 기본적으로 JavaScript Style Guide를 원칙으로 한다

### 라이브러리

- `@woowacourse/mission-utils`에서 제공하는 `Console` API를 사용하여 구현해야 한다.
  - 사용자의 값을 입력 및 출력하려면 `Console.readLineAsync()`와 `Console.print()`를 활용한다.
