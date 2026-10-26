# Product Craft Korea — Agent Guide

이 저장소는 Product Craft Korea의 정적 웹사이트와 GitHub Pages 배포 설정을 관리합니다. 자비스 및 기타 AI 코딩 에이전트는 아래 규칙을 따라 작업합니다.

## Project map

- `index.html`: UI, 스타일, 검색·필터·모달 로직을 포함한 단일 페이지 앱
- `.github/workflows/pages.yml`: `main` 브랜치를 GitHub Pages에 배포하는 워크플로
- `README.md`: 사용법, 연결 구조, 배포 안내
- `LICENSE`: 프로젝트 코드 라이선스

## External connections

- 스킬 메타데이터: `https://raw.githubusercontent.com/RefoundAI/lenny-skills/main/README.md`
- 스킬 원문: `https://github.com/RefoundAI/lenny-skills/tree/main/skills/{slug}`
- 전체 설치: `npx skills add RefoundAI/lenny-skills`
- 개별 설치: `npx skills add RefoundAI/lenny-skills --skill {slug}`

## Working rules

1. 기존 미니멀 편집 디자인과 한국어 인터페이스를 유지합니다.
2. 모바일, 태블릿, 데스크톱 반응형 동작을 보존합니다.
3. 외부 데이터 로딩 실패 시 사용자가 원본 GitHub 저장소로 이동할 수 있는 오류 상태를 유지합니다.
4. 접근성을 위해 키보드 탐색, `aria-label`, 의미 있는 HTML 구조를 유지합니다.
5. 사용자 요청과 관계없는 대규모 리팩터링이나 의존성 추가를 피합니다.
6. Lenny Rachitsky, 게스트, RefoundAI에 대한 출처 귀속을 삭제하지 않습니다.
7. 비밀 키, 토큰, 개인정보를 커밋하지 않습니다.

## Validation

변경 후 다음 항목을 확인합니다.

- `index.html`이 브라우저에서 오류 없이 열리는가
- 원격 README에서 스킬 목록을 파싱하는가
- 검색, 카테고리 필터, 상세 모달, 복사 버튼이 동작하는가
- 570px 및 850px 반응형 레이아웃이 유지되는가
- GitHub Pages 워크플로 YAML이 유효한가

## Deployment

`main` 브랜치에 커밋하면 GitHub Actions의 `Deploy GitHub Pages` 워크플로가 실행됩니다. 저장소 Pages 설정의 Source는 `GitHub Actions`여야 합니다.
