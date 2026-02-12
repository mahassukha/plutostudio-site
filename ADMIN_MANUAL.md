# PLUTO STUDIO 홈페이지 운영/유지보수 매뉴얼 (운영자용)

이 문서는 **비개발자(업로드 가능 수준)** 기준으로 작성되었습니다.

---

## 1) 홈페이지에 접속하기

- 공개 주소(예): `https://www.your-domain.com`
- GitHub 저장소 주소(예): `https://github.com/<username>/<repo>`

---

## 2) “책 표지” 추가하는 방법 (가장 자주 하는 작업)

### 준비물
- JPG/PNG 이미지 1장
- 파일명은 **영문/숫자/언더바** 추천  
  예: `cover_011.jpg`, `my_new_cover.jpg`

### Step A. GitHub 로그인 후 저장소로 이동
1) GitHub 접속 → 로그인  
2) PLUTO STUDIO 저장소(Repository)로 이동

### Step B. `images/` 폴더에 이미지 업로드
1) `images` 폴더 클릭  
2) **Add file → Upload files** 클릭  
3) 새 표지 이미지 파일을 끌어다 놓기(드래그&드롭)  
4) 아래 **Commit changes** 버튼 클릭

### Step C. `covers.json`에 목록 추가 (한 줄 추가)
1) 저장소 루트에서 `covers.json` 클릭  
2) 연필(✏️) 아이콘 **Edit** 클릭  
3) 맨 아래 쪽에 다음 형식으로 한 줄을 추가

예시(마지막 항목 뒤에 콤마 `,` 주의):

```json
{
  "file": "images/cover_011.jpg",
  "title": "Cover 11",
  "category": "Book Cover"
}
```

4) 아래 **Commit changes** 클릭

✅ 완료! 10초~1분 내에 Portfolio 페이지에 반영됩니다.

---

## 3) 표지 순서(정렬) 바꾸기

`covers.json`에서 항목의 순서를 위/아래로 옮기면  
갤러리 표시 순서도 그대로 바뀝니다. (맨 위가 가장 먼저 보임)

---

## 4) 표지 삭제하기

1) `covers.json`에서 해당 항목(파일/제목)을 삭제하고 Commit  
2) `images/` 폴더에서 해당 이미지 파일도 삭제하고 Commit

---

## 5) 소개(About) 페이지 문구 수정

`about.html` 파일을 열고(클릭 → ✏️ Edit)  
텍스트만 수정한 뒤 **Commit changes** 하면 됩니다.

---

## 6) 프로필 사진 교체

1) 새 프로필 사진을 준비 (권장: 정사각형 800x800 내외)  
2) `images/profile.jpg` 파일을 **같은 이름으로 교체 업로드**  
   - GitHub에서 동일 파일명을 업로드하면 “Replace” 형태로 갱신됩니다.

---

## 7) 문의 이메일 수정

`contact.html`과 `about.html`에서 `plutonostudio@gmail.com`을 찾아  
원하는 이메일로 바꾼 뒤 Commit 하면 됩니다.

---

## 8) 도메인(가비아) 연장

- 도메인은 보통 **매년 결제(연장)** 가 필요합니다.
- 가비아 → “My 가비아 / 도메인 관리”에서 연장 결제

---

## 9) 문제가 생겼을 때 체크리스트

- GitHub Pages가 켜져 있는지: Repository → Settings → Pages
- 파일 업로드 후 **Commit**을 눌렀는지
- DNS 연결 직후라면 최대 24시간 기다려보기
- 파일명 오타(대소문자 포함) 확인

---

## 10) 제작자 연락처(옵션)

- 제작: Sam