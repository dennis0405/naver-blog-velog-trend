# SNU AI Challenge 원고 품질 보고서

## Verdict

PASS — 기존 본문을 유지하고 글 말미에 기술 용어 부록을 추가했다. 평가·실험 운영, 모델 학습·메모리, 학습·추론의 세 묶음으로 본문 용어를 설명했다. 최종 순위는 두 원고 모두에 포함하지 않았고 게시를 막는 확인 항목이나 민감정보도 없다.

## Platform Verdicts

- Velog: PASS. 참고 자료 뒤에 Markdown 소제목과 목록으로 용어 부록을 배치했다. 본문 흐름과 결론은 바꾸지 않았다.
- 네이버: PASS. 같은 용어를 짧은 모바일 문단과 목록으로 정리했고 기존 검색형 제목과 설명 흐름을 유지했다.

## Source Draft

- 원본: `posts/drafts/2026-08-11-snu-ai-challenge.md`
- 작업 전 SHA-256: `32894946a4bc3b5f7c8915a1e07616d1a19f85a81f4d52f1fda727d47153ba89`
- 추가 사실 출처: 2026-08-31 사용자 직접 제공 내용
- 원본 초안은 수정하지 않았으며 작업 전후 SHA-256이 일치한다.

## Technical Accuracy

- 와플스튜디오 AI 스터디에서 서울대학교 학부생 3명이 팀을 구성했다는 참여 맥락을 양쪽에 추가했다.
- AI 논문 스터디를 계획했다가 대회 기반의 경험형 스터디로 방향을 바꿨다는 동기를 보존했다.
- 작성자의 역할은 기존 근거에 맞춰 멀티모달 모델 설계와 학습·추론 실험으로 한정했다. 다른 팀원의 역할은 추정하지 않았다.
- `0.86585`는 작성자가 수행한 실험에서 확인한 최고 public leaderboard Exact Match로만 설명했다. 최종 순위는 언급하지 않았다.
- 개최 배경, 2026년 과제, 평가 방식, 참여 기간, TPRU-7B·InternVL2.5-8B-MPO·Qwen3.5-9B의 비교 조건과 점수를 유지했다.
- MultiHead 구성, 순열 채점식, constrained decoding, Token Attention, TTA, Frontier 계열, RL 회고와 27B 결과를 보존했다.
- 복합 실험의 개별 기여를 분리하지 못했다는 한계와 세 모델만으로 선형 관계를 단정할 수 없다는 유보를 유지했다.
- 부록은 본문에 등장하는 public leaderboard, Exact Match Accuracy, benchmark, development/validation set, checkpoint, ablation의 개념을 설명한다.
- Backbone·QLoRA·NF4 4-bit·adapter·token·pooling·attention·head와 TTA·Multi-Turn verification·constrained decoding 등 빠르게 등장한 용어를 글의 실험 맥락에 맞춰 설명한다.
- 본문에서 이미 자세히 소개한 모델의 성능이나 대회 결과는 부록에서 새로 해석하지 않았다.

## Cross-Platform Factual Parity

- 참여 동기, 소속 맥락, 팀 규모, 작성자 역할, 점수 범위가 두 원고에 모두 있다.
- 날짜, 모델명, 실험명, 수치, 인과관계, 참고 URL과 결론이 두 원고에서 일치한다.
- 최종 순위와 팀원 개인정보는 두 원고 모두에 없다.
- 부록의 용어 묶음과 대회별 예시는 두 원고에서 일치한다.
- 플랫폼 차이는 제목·소제목·문단 호흡과 Markdown 표현뿐이다.
- `must_include` 6개 항목을 양쪽 원고에서 모두 확인했다.

## Originality

- 기존 기술 사실은 사용자 초안에서, 참여 맥락과 부록 추가 지시는 사용자가 직접 제공한 내용에서 가져왔다.
- 부록은 본문에 이미 등장하는 표준 기술 용어를 일반적인 개념 수준에서 풀었고 새로운 실험 결과나 수치를 추가하지 않았다.
- 2026-08-31 공통·Velog·네이버 playbook에서는 추상적인 편집 규칙만 사용했다.
- 스타일 추출에 쓰인 외부 본문이나 표현은 사용하지 않았다.

## Confidentiality

- API token·private key·이메일·IPv4 패턴: 0건
- 비공개 저장소·서버 정보·credential·공개 여부가 불분명한 대회 데이터: 발견되지 않음
- 팀 정보는 인원 수와 학부생·동아리 맥락만 공개했으며 팀원 신원과 역할은 포함하지 않음

## Style Playbooks

- 공통: 회고의 결론과 참고 자료 뒤에 부록을 분리해 기술 용어 설명이 본문 흐름을 끊지 않게 했다.
- Velog: 세 개의 하위 소제목과 Markdown 목록으로 용어를 빠르게 찾아볼 수 있게 했다.
- 네이버: 같은 개념을 짧은 정의 문장으로 구성해 모바일 편집기에 옮기기 쉽게 했다.
- Velog 표본이 3건뿐인 점을 고려해 low-confidence 장식 규칙은 강제하지 않았다.

## Humanize Korean

- Velog와 네이버를 H2 경계에서 각각 5,000자 이하 청크로 나눠 별도 Fast Path로 검토했다. 부록을 포함해 건너뛴 절은 없고 모든 청크가 자체검증을 통과했다.
- Velog: 변경률 `0.000%`, 등급 B, 자체검증 6/6. 새 정의가 이미 짧고 직접적이어서 의미 보존을 우선해 추가 윤문하지 않았다.
- 네이버: 변경률 `0.000%`, 등급 B, 자체검증 6/6. 모바일용 정의의 기술 식별자와 의미를 그대로 보호했다.
- URL, 표, 코드, 날짜, 수치, 고유명사, 기술 식별자와 인과관계는 보호했다.

## Publishing Format

- `post.velog.md`: H1 1개, 일관된 heading 계층, 닫힌 code fence, Markdown 링크·표와 말미 용어 부록 보존.
- `post.naver.txt`: 제목으로 시작하는 UTF-8 일반 텍스트이며 Markdown heading·fence·inline backtick이 없다.
- 두 출력 모두 내부 메타데이터, `HUMANIZE-SUMMARY`, 최종 순위와 `[확인 필요]` 표시가 없다.

## Remaining TODO

- 필수 TODO 없음.
- 게시된 글에 반영하기 전 Velog 편집 화면에서 부록의 위치와 목록 가독성을 최종 확인하면 된다.
