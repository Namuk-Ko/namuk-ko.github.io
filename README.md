# namuk-ko.github.io

Namuk Ko 이력 사이트. Hugo로 빌드하고 GitHub Actions로 GitHub Pages에 배포한다.

## 내용 수정

모든 내용은 `data/*.yml`에 있다. 템플릿은 건드리지 않아도 된다.

| 파일 | 섹션 |
|---|---|
| `data/Profile.yml` | 첫 화면 문구, 연락 링크, 핵심 수치 |
| `data/Summary.yml` | Summary |
| `data/Experience.yml` | Experience (문장 안 `**수치**`는 강조 표시) |
| `data/Projects.yml` | Projects (문제 · 판단 · 결과, 데이터 흐름) |
| `data/Skills.yml` | Skills |
| `data/Education.yml` | Education |
| `data/Publications.yml` | Publications |

## 로컬 미리보기

```bash
hugo server
```

`http://localhost:1313`에서 확인한다. 파일을 저장하면 바로 반영된다.

## 배포

`main`에 push하면 `.github/workflows/hugo.yml`이 빌드·배포한다. 저장소 Settings > Pages의 Source는 "GitHub Actions"여야 한다.

## 구조

- `layouts/index.html`, `layouts/partials/`: 페이지 템플릿
- `assets/css/style.css`: 스타일 (다크 테마, 인쇄 시 라이트)
- `static/assets/img/`: 이미지
