# base-resume

HTML · CSS만으로 만든 이력서 웹페이지 템플릿입니다.
`index.html`의 **글자만** 바꾸면 나만의 이력서 사이트가 완성됩니다.

## 파일 구성

| 파일 | 역할 |
| --- | --- |
| `index.html` | 이력서 본문과 프로젝트 목록 |
| `project-azure-ml.html` | Azure ML 이미지 분류 프로젝트 상세 페이지 |
| `project-rag-chatbot.html` | RAG 챗봇 프로젝트 상세 페이지 |
| `project-customer-ai.html` | 고객 문의 분류 프로젝트 예시 상세 페이지 |
| `project-demand-forecast.html` | 매출 수요 예측 프로젝트 예시 상세 페이지 |
| `style.css` | 전체 페이지 디자인 |
| `profile.svg` | 프로필 이미지 (내 사진으로 교체 가능) |
| `.github/workflows/ci.yml` | push 할 때 HTML 문법 자동 검사 |
| `.htmlvalidate.json` | HTML 검사 규칙 설정 |

## 수정 · 배포 6단계

1. **내용 수정** — 이력서와 프로젝트 목록은 `index.html`, 프로젝트 상세 내용은 해당 `project-*.html` 파일에서 수정합니다. 태그(`<h3>`, `</li>` 등)는 지우지 마세요.
2. **더블클릭으로 확인** — `index.html`을 더블클릭해 브라우저에서 화면을 확인합니다.
3. **커밋** — `git add .` → `git commit -m "이력서 내용 수정"`
4. **push** — `git push`
5. **Actions 확인** — GitHub 저장소의 **Actions** 탭에서 "HTML 검사"가 초록색 ✅ 인지 확인합니다.
6. **Vercel 배포** — [vercel.com](https://vercel.com) 에서 **Add New → Project → 내 저장소 Import → Deploy** 를 누릅니다. (설정 변경 없이 그대로 배포)

> 💡 **CI가 빨간색 ❌ 이면:** Actions 로그의 **첫 번째 error** 줄에서 `46:12` 처럼 표시된 앞 숫자가 **줄 번호**(46번째 줄)이니, 에디터에서 그 줄의 빠진 태그를 확인합니다.

## 프로필 사진 바꾸기

사진 파일(예: `me.jpg`)을 이 폴더에 넣고, `index.html`의 `src="profile.svg"`를 `src="me.jpg"`로 바꿉니다.

> 편입 이력과 추가된 두 프로젝트는 화면 구성용 예시입니다. 공개하기 전에 본인의 실제 학교, 기간, 프로젝트 내용으로 바꿔 주세요.

## 주의

전화번호 · 주소 · 생년월일 · 이메일 같은 개인정보는 공개 사이트에 올리지 마세요.
