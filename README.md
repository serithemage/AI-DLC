# AI-DLC (AI-Driven Development Lifecycle) 방법론 한국어 번역

> **원본 문서:** [AI-Driven Development Lifecycle](https://prod.d13rzhkk8cj2z0.amplifyapp.com/) by Raja SP, Amazon Web Services

AI 주도 개발 생명주기(AI-DLC) 방법론 정의서의 한국어 번역 문서입니다.

## AI-DLC란?

AI-DLC는 기존 SDLC/애자일 방법론을 AI 시대에 맞게 **제1원칙에서 재구상** 한 AI 네이티브 개발 방법론입니다. AI를 단순한 보조 도구가 아닌 개발 프로세스의 중심 협력자로 배치하여, 워크플로우 조율부터 작업 분해, 코드 생성, 테스트, 배포까지 전 과정을 AI가 주도하고 인간이 검증하는 패러다임을 제시합니다.

## 핵심 개념

| 기존 방법론 | AI-DLC | 설명 |
|---|---|---|
| 에픽/서브도메인 | **유닛(Unit)** | 응집력 있는 자체 포함된 작업 요소 |
| 스프린트 | **볼트(Bolt)** | 시간/일 단위의 신속한 반복 주기 |
| 수동 요구사항 정의 | **몹 엘라보레이션(Mob Elaboration)** | AI 주도의 협업적 요구사항 정교화 의식 |
| 수동 개발 | **몹 구성(Mob Construction)** | AI 주도의 협업적 구현 의식 |

## 3단계 프레임워크

```
인셉션(Inception) → 구성(Construction) → 운영(Operations)
```

- **인셉션 단계:** 의도(Intent) 포착 및 유닛으로 분해
- **구성 단계:** 도메인 설계 → 논리 설계 → 코드 생성 → 테스트/검증
- **운영 단계:** 배포, 관찰 가능성, AI 기반 사전 문제 해결

## 10대 핵심 원칙

1. 개조가 아닌 재구상
2. 대화 방향의 역전 (AI가 주도, 인간이 검증)
3. 설계 기법의 핵심 통합 (DDD, BDD, TDD)
4. AI 역량과의 현실적 정렬
5. 복잡한 시스템 구축 지원
6. 인간 공생을 향상시키는 것 유지
7. 친숙함을 통한 전환 촉진
8. 효율성을 위한 책임 간소화
9. 단계 최소화, 흐름 극대화
10. 고정된 SDLC 워크플로우 없음

## 문서 구조

```
.
├── AI-Driven Development Liftcycle.md   # 원본 번역 문서
├── index.md                              # GitHub Pages용 (동일 내용)
├── _config.yml                           # Jekyll 설정
└── images/                               # 다이어그램 이미지
    ├── ai-dlc-framework.png
    ├── ai-dlc-workflow.png
    └── ai-dlc-detailed-workflow.png
```

## GitHub Pages

이 문서는 GitHub Pages로 호스팅됩니다: https://serithemage.github.io/AI-DLC/

## 저작권

본 문서의 모든 권리는 원 저작자(Raja SP, Amazon Web Services)에게 있습니다. 이 저장소는 원본을 한국어로 번역한 것입니다.
