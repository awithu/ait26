# IT 블로그

GitHub Pages를 사용한 Jekyll 기반 IT 기술 블로그입니다.

## ⚠️ 개인정보 보호

**절대 커밋하면 안 되는 정보:**
- 실제 이메일 주소 (example.com, noreply 제외)
- 비밀번호, API 키, 토큰
- 전화번호, 주소 등 개인정보
- 민감한 설정 파일 (.env, secrets.yml 등)

**자동 보호 기능:**
- Pre-commit hook이 커밋 전에 개인정보를 자동으로 검사합니다
- 민감한 정보가 감지되면 커밋이 차단됩니다
- `.gitignore`에 민감한 파일 패턴이 포함되어 있습니다

**이메일 주소 사용 시:**
- 실제 이메일 대신 `your.email@example.com` 사용
- 또는 GitHub의 noreply 이메일 사용: `username@users.noreply.github.com`

## 로컬에서 실행하기

1. Ruby와 Bundler 설치
2. 의존성 설치:
   ```bash
   bundle install
   ```
3. 로컬 서버 실행:
   ```bash
   bundle exec jekyll serve
   ```
4. 브라우저에서 `http://localhost:4000/ait26` 접속

## 새 글 작성하기

`_posts/` 디렉토리에 다음 형식으로 파일을 생성하세요:

```
YYYY-MM-DD-제목.md
```

예시:
```
2024-01-15-자바스크립트-기초.md
```

## GitHub Pages 배포

1. 코드 커밋 및 푸시:
   ```bash
   git add .
   git commit -m "Initial blog setup"
   git push origin master
   ```

2. GitHub 저장소 Settings → Pages에서:
   - Source: Deploy from a branch
   - Branch: master 선택
   - Save

3. 몇 분 후 `https://danielseol9250.github.io/ait26`에서 확인 가능

## 포스트 작성 형식

```markdown
---
layout: post
title:  "포스트 제목"
date:   YYYY-MM-DD HH:MM:SS +0900
categories: [카테고리1, 카테고리2]
tags: [태그1, 태그2, 태그3]
---

# 제목

내용...
```

