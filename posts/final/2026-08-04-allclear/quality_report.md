# 애플 개발자 계정 이전 원고 품질 보고서

## Verdict

PASS — Velog와 네이버 게시본 모두 초안의 작업 순서·수치·불확실성을 보존했으며, 공개 제외 항목과 게시 형식을 통과했다.

## Platform Verdicts

- Velog: PASS. Markdown 헤딩, 코드 블록, 표, 링크를 보존했고 각 예제 앞뒤에 목적과 해석이 있다.
- 네이버: PASS. 네이버 편집기에 붙여넣을 수 있는 일반 텍스트로 변환했으며, 검색형 제목과 짧은 문단 흐름을 적용했다.

## Source Draft

- 원본: `posts/drafts/2026-08-04-allclear.md`
- 원본 SHA-256: `8a9d7ca2596c93a7b576b15d2da08f68168c812e5ca0f721c56843af956d93e7`
- 검토 과정에서 원본 초안을 수정하지 않았다.

## Technical Accuracy

- 기간, 담당 범위, `old_sub -> transfer_identifier -> new_sub` 순서, 60일 기한, 실패 로그와 검증 결과를 유지했다.
- SQL, API 요청, 로그인 fallback, iOS 서명·entitlement 예제와 참고 URL 3개를 초안 범위 안에서 보존했다.
- `invalid_client`의 Apple 내부 원인은 확인하지 못했다는 유보를 유지했다.
- 외부 사실을 새로 추가하거나 수치·원인을 추정하지 않았다.

## Cross-Platform Factual Parity

- 두 게시본의 절 순서, 코드·설정, 실패 사례, 결과, 참고 자료가 일치한다.
- 플랫폼 차이는 제목과 Markdown 표현 방식뿐이며 기술적 결론은 같다.

## Originality

- 원고의 사실 자료는 사용자 초안만 사용했다.
- 공통·Velog·네이버 playbook에서는 제목, 구조, 문단 리듬, 목록·코드 배치 같은 추상 규칙만 적용했다.
- 스타일 추출에 사용된 외부 블로그 본문이나 표현은 사용하지 않았다.

## Confidentiality

- 서비스명 `올클(AllClear)`은 사용자가 공개를 요청한 범위로 포함했고, 저장소 링크는 0건이다.
- 실제 Team ID·Key ID·private key: 0건
- 운영 DB 접속 정보·개인 이메일·사용자 식별자·정확한 내부 계정 수: 0건
- `.p8`, client secret, Team ID 등은 설명용 명칭이나 placeholder로만 남겼다.

## Style Playbooks

- 2026-08-31 추출본의 공통·Velog·네이버 playbook을 적용했다.
- Velog는 실제 문제를 도입에서 바로 제시하고, 문제 → 확인 → 조치 → 검증 흐름을 Markdown 소제목으로 나눴다.
- 네이버는 핵심 기술을 앞세운 검색형 제목을 사용하고 Markdown 기호를 편집기 친화적인 일반 텍스트로 변환했다.
- 비교 축이 명확한 표와 재현·판단에 필요한 코드만 유지했다.

## Humanize Korean

- Velog와 네이버 본문을 플랫폼별로 다시 점검했다.
- 보호 대상: 코드, 표의 값, URL, 식별자 placeholder, 수치, 인과관계, 불확실성 표현.
- 과장된 괄호 문구와 느낌표를 제거하고, 한 문단에 하나의 판단이나 작업만 남겼다.
- 자동 지표: Velog `low`, 네이버 `low`.

## Publishing Format

- `post.velog.md`: H1 1개, 일관된 H2/H3, Markdown 코드·표·링크 보존.
- `post.naver.txt`: Markdown 헤딩·인라인 코드 표식을 제거한 UTF-8 일반 텍스트.

## 2026-08-31 Published Post Revision

- Second Brain의 공개 가능한 프로젝트 설명과 사용자가 직접 다듬은 네이버 게시본을 참고해 도입부를 보완했다.
- 올클을 서울대학교 동아리 목록·모집공고·활동 후기를 한곳에서 제공하는 서비스로 소개했다.
- `운영 중인 동아리 탐색 iOS 앱`을 `올클 iOS 앱`으로 구체화하고, WaffleStudio 계정으로의 이전 맥락을 명시했다.
- 긴 도입 문단을 나눠 문제 전환이 자연스럽게 이어지도록 조정했다.
- 기술 절차, 수치, 코드, 실패 사례와 결론은 변경하지 않았다.

## Remaining TODO

- 필수 TODO 없음.
- 공개 URL에서 새 도입부, 주요 H2, 참고 자료와 썸네일이 각각 1회 렌더링되는 것을 확인했다.
- 수정 중 발견한 CodeMirror 본문 중복 문제와 재발 방지 절차는 `posts/results/2026-08-31-velog-republish.md`에 기록했다.
