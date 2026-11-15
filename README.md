# Mobile App User Flow

모바일 앱의 첫 실행부터 첫 유용한 결과와 핵심 화면 이동까지 설계하는 재사용 가능한 스킬입니다. 쇼핑, 여행, 학습 등 앱의 목적에 맞춰 질문, 체험, 가입, 권한 요청의 순서를 결정합니다.

## 사용 방법

이 저장소의 `SKILL.md`를 내려받아 Codex 개인 스킬 폴더의 `mobile-app-user-flow/SKILL.md`로 저장하세요.

예를 들어 개인 스킬 폴더가 `~/.codex/skills`인 환경에서는 `~/.codex/skills/mobile-app-user-flow/SKILL.md`에 저장합니다. 사용자 지정 `CODEX_HOME`을 사용하는 환경에서는 해당 폴더 아래 `skills`에 저장합니다.

새 채팅에서 다음과 같이 요청할 수 있습니다.

```text
$mobile-app-user-flow를 사용해 여행 일정 앱의 첫 실행부터 첫 일정 저장까지 설계해줘.
```

## Claude Code에서 사용하기

Claude Code용으로 조정한 스킬은 `.claude/skills/mobile-app-user-flow/SKILL.md`에 있습니다. 원본 지침에 슬래시 명령 인자, 결과 정리 형식(Mermaid 흐름도·화면별 표), 구현 전 코드 탐색, 실행 검증 방법을 더했습니다.

- **이 저장소 안에서**: 별도 설치 없이 프로젝트 스킬로 자동 인식됩니다.
- **모든 프로젝트에서(개인 스킬)**: 아래 명령으로 복사합니다.

```bash
mkdir -p ~/.claude/skills/mobile-app-user-flow && cp .claude/skills/mobile-app-user-flow/SKILL.md ~/.claude/skills/mobile-app-user-flow/
```

호출 예시:

```text
/mobile-app-user-flow 여행 일정 앱의 첫 실행부터 첫 일정 저장까지 설계해줘
```

온보딩, 가입·권한 시점, 화면 흐름 설계를 요청하면 Claude가 자동으로 스킬을 불러오기도 합니다.

## 포함된 내용

- 사용자가 처음 얻을 유용한 결과와 진입점 정의
- 선택 질문과 건너뛰기, 기능 체험 설계
- 가입·권한·결제 시점과 복귀 경로 정의
- 로딩, 실패, 재시도와 앱 재실행 동작 점검
- 직접 확인한 동작과 미확인 흐름 구분

스킬에 포함된 플랭 사례는 온보딩에서 직접 관찰한 화면 전환만 다룹니다. 회원가입 이후 홈과 학습 및 결제 동선은 미확인입니다.

저장소에는 재사용 가능한 지침과 사용 안내를 담았습니다. 개인 계정 정보, 기기 식별자, 스크린샷, 연결 로그는 포함하지 않습니다.
