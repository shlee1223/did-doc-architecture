# 커밋 메시지 가이드라인

## 1. 커밋 메시지 구조

기본적으로 제목 / 본문 / 꼬리말로 구성하고 한 줄의 공백을 두어 구분

- **type**: 해당 커밋은 무엇에 대한 작업인지 키워드를 통해 표시
- **subject**: 커밋메시지의 제목
- **body**: 커밋메시지의 본문 (선택사항)
- **footer**: 커밋메시지의 맺음말 (선택사항)

```c#
Type: Subject

Body

Footer
```

### 1.1. type

- **feat**: 새로운 기능 추가
- **fix**: 버그 수정
- **build**: 빌드 관련 파일 수정
- **ci**: CI관련 설정 수정
- **docs**: 문서(문서 추가, 수정, 삭제)
- **style**: 스타일(코드 형식, 세미콜론 추가: 비즈니스 로직에 변경 없는 경우)
- **refactor**: 코드 리팩토링
- **test**: 테스트(테스트 코드 추가, 수정, 삭제: 비즈니스 로직에 변경 없는 경우)
- **chore**: 기타 변경사항(빌드 스크립트 수정 등)

### 1.2. subject

- 영문으로 작성된 제목은 50자를 넘지 않으며, 마침표를 사용하지 않음
- 제목에는 커밋 타입을 포함함
- 명령 조를 사용하여 과거 시제 대신 현재 시제를 사용함
- 제목과 본문은 한 줄을 띄워 구분함
- 제목의 첫 글자는 대문자로 시작함
- 이슈 관련 내용이라면 이슈 번호를 제목에 포함함

예시: 영문 제목 케이스
```c#
# Add : 추가
# Remove : 삭제
# Simplify : 단순화
# Update : 보완
# Implement : 구현
# Prevent : 방지
# Move : 이동
# Rename : 이름 변경
```

### 1.3. body

- 한 줄에 72자를 넘기지 않음
- 어떻게(How)보다 무엇을, 왜(What, Why)에 맞춰 작성
- 설명, 커밋의 이유를 작성할 때 필요

### 1.4. footer

- 어떤 이슈에서 왔는지 같은 **참조 정보들을 추가**하는 용도로 사용

### 1.5. 예시

```c#
feat: Summarize changes in around 50 characters or less 
More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789

```

### 1.6. 정리

| Type | Subject | Body (선택 사항) | Footer (선택 사항) |
|------|---------|------------------|---------------------|
| feat: 새로운 기능 추가 | 제목은 최대 50글자를 넘기지 않는다. | 본문은 한 줄당 72자 내로 작성한다. | 이슈 트래커 ID를 작성한다. |
| fix: 버그 수정 | 마침표 및 특수기호는 사용하지 않는다. | 양에 구애받지 않고 최대한 상세히 작성한다. | "유형: #이슈 번호" 형식으로 작성한다. |
| docs: 문서 수정 | 영문으로 표기하는 경우 동사 원형을 가장 앞에 두고 첫 글자는 대문자로 표기한다.(과거 시제 사용 금지) | 어떻게 변경했는지 보다 무엇을 변경했는지 또는 왜 변경했는지를 설명한다. | 여러 개의 이슈 번호를 적을 때는 쉼표(,)로 구분한다. |
| style: 코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우 | | | Fixes: 이슈 수정 중 (아직 해결되지 않은 경우) |
| refactor: 코드 리팩토링 | | | Resolves: 이슈를 해결한 경우 |
| test: 테스트 코드, 리팩토링 테스트 코드 추가 | | | Ref: 참고할 이슈가 있을 경우 |
| chore: 빌드 업무 수정, 패키지 매니저 수정, production code와 무관한 부분들 (.gitignore, build.gradle 같은) | | | Related to: 해당 커밋에 관련된 이슈 번호(아직 해결되지 않은 경우) |
| comment: 주석 추가 및 변경 | | | ex) Fixes: #45 Related to: #34, #23 |
| remove: 파일, 폴더 삭제 | | | |
| rename: 파일, 폴더명 수정 | | | |

## 2. 예약 키워드 사용

### 2.1. 예약 키워드

커밋 메시지를 영어로 작성할 때 예약된 키워드가 있다면 특정 기능이 동작하도록 하는데
아래와 같은 키워드를 사용하여 이슈를 자동으로 종료하는 방법이 있으며 예약된 키워드는
커밋 메시지의 어느 위치에 있어도 동작함

- **fix / fixes /fixed**
  - 코드 변경과 연관된 이슈 해결에 사용됨
  - 주로 버그 수정이나 기능 변경과 관련된 이슈를 해결할 때 사용
- **resolve / resolves / resolved**
  - 코드 변경과는 직접적인 연관이 없는 이슈를 처리하는 데 사용
  - 주로 기술적인 문제 해결이나 요구 사항 충족을 위한 이슈 해결에 사용
- **close / closes / closed**
  - 이슈를 닫을 때 사용
  - 위의 두 키워드보다 더 일반적이며, 코드 변경과 관계 없이 이슈를 완료하거나 해결할 때 사용

### 2.2. 예시

- 커밋 후 브랜치를 푸시하면 아래 메시지로 이슈가 자동으로 종료
- 이슈 종료는 커밋이 속한 브랜치에 따라 달라짐
- 기본 브랜치가 **master**인 경우
  - master 브랜치에서 커밋 후 원격 서버로 푸시하면 해당 이슈가 종료
  - 다른 브랜치에서 커밋하면 추후 원격 서버의 master 브랜치에 머지될 때 이슈가 종료

```c#
# 제목에 이슈 한 개 닫기를 적용한 사례
Close #31 - refactoring wrap-up

* This is wrap-up of refactoring main code.
* main.c
  * removed old comments
  * fixed rest indentations
  * method extraction at line no. 35

# 본문에 이슈 여러 개 닫기를 적용한 사례
Update policy 16/04/02

* This closes #128 - cab policy, closes #129 - new hostname, and fixes #78 - bug on logging.
* cablist.txt: changed ACL due to policy update delivered via email on 16/04/02, @mr.parkyou
* hostname.properties: cab hostname is updated
* BeautifulDeveloper.java: logging problem on line no. 78 is fixed. The `if` statement is never happening. This deletes the `if` block.
```