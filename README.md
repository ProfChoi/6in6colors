# 📖 에세이 집 진도 현황 대시보드

6인 공동 에세이 프로젝트의 집필 진도를 한눈에 파악하고 관리하는 대시보드입니다.

## ✨ 주요 기능

- **가로형 대시보드 테이블** — 참여자 6명을 행(row)으로, 월별 작업을 열(column)로 배치해 한눈에 전체 현황 파악
- **클릭으로 완료 체크** — 각 항목을 클릭하면 체크/해제 토글
- **신호등 표시** — 빨간불(미시작) → 노란불(진행 중) → 초록불 반짝임(개인 작업 완료)
- **7~9월 통합 섹션** — 마무리 정리·출판 준비·출간 완료는 전체 공통 작업으로 하단에 별도 표시
- **전체 진도 바** — 개인 작업 + 공통 작업 포함 전체 진행률 표시
- **URL 공유 기능** — 현재 진도 상태가 URL 해시에 저장되어 링크 하나로 공유 가능

## 📅 일정

| 기간 | 작업 |
|------|------|
| 2026년 2월 | 목차 완성 |
| 2026년 3월 | 에세이 1·2편 완성 |
| 2026년 4월 | 에세이 3·4편 완성 |
| 2026년 5월 | 에세이 5·6편 완성 |
| 2026년 6월 | 에세이 7·8편 완성 |
| 2026년 7~9월 | 마무리 정리 · 출판 준비 · 출간 (통합) |

---

## 🚀 GitHub Pages 배포 방법

### 1단계: GitHub 저장소 생성

1. [github.com/new](https://github.com/new) 에서 새 저장소 생성
2. 저장소 이름 예시: `essay-progress-dashboard`
3. **Public** 으로 설정 (GitHub Pages 무료 이용)
4. **Create repository** 클릭

### 2단계: 파일 업로드

방법 A — 웹 브라우저에서 직접 업로드:
1. 생성한 저장소 페이지에서 **Add file → Upload files** 클릭
2. `index.html` 파일을 드래그하여 업로드
3. **Commit changes** 클릭

방법 B — Git 명령어 사용:
```bash
git init
git add index.html README.md
git commit -m "에세이 진도 대시보드 추가"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/essay-progress-dashboard.git
git push -u origin main
```

### 3단계: GitHub Pages 활성화

1. 저장소 페이지 → **Settings** 탭 클릭
2. 왼쪽 메뉴에서 **Pages** 클릭
3. **Source** → `Deploy from a branch` 선택
4. **Branch** → `main`, 폴더 → `/ (root)` 선택
5. **Save** 클릭

약 1~2분 후 아래 형식의 URL로 접근 가능:
```
https://YOUR_USERNAME.github.io/essay-progress-dashboard/
```

---

## 📱 사용 방법

### 진도 체크하기
- 각 참여자 카드에서 완료한 항목을 클릭하면 체크 표시
- 다시 클릭하면 해제

### 팀원과 진도 공유하기
1. 진도를 체크한 뒤 상단의 **🔗 진도 URL 복사** 버튼 클릭
2. 복사된 URL을 카카오톡, 이메일 등으로 팀원에게 공유
3. 팀원이 해당 URL을 열면 현재 진도가 그대로 보임

> **📌 URL 공유 방식 설명**
> 진도 데이터는 URL의 `#` 뒷부분에 저장됩니다.
> 예: `https://...github.io/.../#WzAsOCwxMiwwLDUsM10=`
> 이 URL을 공유하면 서버 없이도 현재 상태를 팀원과 공유할 수 있습니다.

### 신호등 색상 의미
| 색상 | 상태 |
|------|------|
| 🔴 빨간불 | 아직 시작하지 않은 상태 |
| 🟡 노란불 | 일부 완료, 진행 중 |
| 🟢 초록불 (반짝임) | 12개 항목 모두 완료! |

---

## 💡 권장 활용 방법

1. **코디네이터(관리자)** 한 명이 대시보드 URL을 북마크
2. 팀원에게 진도 보고를 받을 때마다 항목 체크
3. 체크 후 **🔗 진도 URL 복사** → 단체 대화방에 붙여넣기
4. 팀원 모두가 최신 URL을 열어 전체 진도 확인

---

## 🛠️ 기술 정보

- 순수 HTML/CSS/JavaScript — 별도 서버, 데이터베이스 불필요
- 진도 데이터: URL 해시 + 브라우저 로컬스토리지 이중 저장
- 폰트: Noto Sans KR (Google Fonts)
- GitHub Pages로 무료 호스팅 가능
