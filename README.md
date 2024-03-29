# vite를 이용한 포트폴리오 사이트 만들기

## vite를 사용하는 이유

[vite](https://ko.vitejs.dev/guide/)

1. 빠른 개발 서버: 실시간으로 코드를 수정하고 브라우저에 반영

2. 모듈화 지원: Vite는 ES 모듈을 기본으로 사용, 최신 브라우저에서 빠르게 로딩.

3. 플러그인 생태계: Vite는 다양한 플러그인을 지원, 확장 가능

4. Vue.js와의 통합: Vue.js 프로젝트의 개발을 더 쉽게 만듭니다.

5. 빌드 최적화: Vite는 빌드 시스템도 제공하며, 최적화된 번들을 생성하여 프로덕션 환경에서 빠른 성능을 제공합니다.

6. TypeScript 지원: TypeScript를 네이티브로 지원

7. 경량화 및 간결한 설정: 간결한 설정 파일 사용, 필요한 설정 최소화

8. 현대적인 생태계: 최신의 프론트엔드 개발 트렌드와 도구를 반영, 현대적이고 생산적인 환경을 제공

## 구현 기능

- 구글 폰트 적용
- smooth 효과 : https://lenis.studiofreight.com/
- 자바스크립트 메뉴 클릭 이동 효과
- GSAP를 이용한 가로 효과
- JavaScript 모듈 기능 적용
- 웹표준 준수를 위한 스킵 메뉴 및 aria, role 적용
- vite 빌드 작업 `npm run build`
- netlify 배포

## vite 명령어

프로젝트 만들기 : `npm create vite@latest`
프로젝트 실행 : `npm run dev`

## 초기 설정

1. vite.config.js로 시작페이지 설정을 바꿔줌.

2. git 연동
   git init
   git add README.md
   git commit -m "first commit"
   git branch -M main
   git remote add origin https://github.com/SeoEugene/vite-project.git
   git push -u origin main

## 트러블 슈팅

- git 업로드 error
  On branch main
  Changes not staged for commit:
  (use "git restore <file>..." to discard changes in working directory)
  modified: README.md

Untracked files:
(use "git add <file>..." to include in what will be committed)
.gitignore
package-lock.json
package.json
vite.config.js

### 주소 다시 셋팅

나의 git 주소 : https://github.com/SeoEugene/vite-project.git

git remote set-url origin https://SeoEugene@github.com/SeoEugene/vite-project.git

git push -u origin master

### git에서 먼저 만든 저장소를 가져올때

git pull {원격저장소별칭 보통 origin이라고 함} master

### 새로운 데이터를 업데이트 시킬 때

git push {원격저장소 별칭 보통 origin} master
