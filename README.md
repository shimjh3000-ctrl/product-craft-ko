# Product Craft Korea

첨부 레퍼런스의 미니멀 편집 디자인을 바탕으로 만든 한국어 반응형 제품 리더십 스킬 라이브러리입니다.

## 연결 구조

- **웹사이트:** 이 저장소의 GitHub Pages로 자동 배포
- **스킬 데이터:** `RefoundAI/lenny-skills`의 최신 README를 브라우저에서 실시간 로드
- **AI Agent:** 전체 또는 개별 스킬의 `npx skills add` 명령 제공
- **원문:** 각 스킬 카드에서 GitHub의 해당 `SKILL.md` 폴더로 이동

## 주요 기능

- 76개 스킬 검색
- 13개 카테고리 필터
- 스킬 상세 모달
- 전체/개별 설치 명령 복사
- 모바일·태블릿·데스크톱 반응형 UI
- GitHub Pages 자동 배포 워크플로

## 로컬 실행

`index.html`을 브라우저에서 열거나 정적 서버를 실행하세요.

```bash
python -m http.server 8080
```

## GitHub Pages

저장소의 **Settings → Pages → Build and deployment → Source**를 **GitHub Actions**로 한 번 설정하면, `main` 브랜치 변경 시 자동 배포됩니다.

## 출처와 권리

스킬 구조와 메타데이터는 [RefoundAI/lenny-skills](https://github.com/RefoundAI/lenny-skills)를 사용합니다. 저장소 구조는 MIT 라이선스이며, 기저 인사이트·인용·프레임워크의 권리는 Lenny Rachitsky와 각 게스트에게 있습니다.
