# Git Commit 메시지 작성 가이드

커밋 메시지는 **짧고 명확하게 변경 내용을 표현**하는 것이 핵심입니다. 특히 협업 환경에서는 일관된 컨벤션을 지키는 것이 중요합니다.

---

## 1. 기본 구조

커밋 메시지는 일반적으로 **세 부분**으로 나눌 수 있습니다:

```
<타입>(<옵션>): <제목>
<빈 줄>
<상세 설명>
```

* **타입 (type)**: 변경의 성격을 나타냄

  * `feat`: 새로운 기능 추가
  * `fix`: 버그 수정
  * `chore`: 빌드, 설정, 기타 잡일
  * `docs`: 문서 변경
  * `style`: 코드 포맷, 세미콜론 누락 등 기능 변경 없는 스타일
  * `refactor`: 코드 리팩토링 (기능 변경 없음)
  * `test`: 테스트 관련 추가/수정
* **옵션 (scope)**: 변경 영역 (선택)
* **제목 (subject)**: 변경 내용 요약 (50자 이내 권장)

---

## 2. 작성 예시

### 초기 구조 세팅

```
chore: initial manifest v3 setup with background service worker
```

### 새 기능 추가

```
feat: setup basic popup UI and storage.local for shortcuts
```

### 버그 수정

```
fix: resolve issue with popup not loading stored shortcuts
```

### 코드 리팩토링

```
refactor: simplify background.js event listener logic
```

---

## 3. 작성 팁

1. **명령문 현재형** 사용: `add`, `fix`, `update` 등
2. **짧고 명확하게**: 제목은 50자 이내, 본문은 72자 내외
3. **본문 작성 시**:

   * 변경 이유와 상세 내용 작성
   * 필요한 경우 관련 이슈 번호 포함 (#1, #2 등)

---

## 4. 권장 커밋 메시지 예시 모음

```
chore: initial project setup with manifest v3
feat: add storage.local integration for shortcuts
feat: implement popup UI with tabbed categories
fix: correct background service worker event registration
refactor: reorganize JSON structure for shortcut data
docs: add README with installation instructions
```
