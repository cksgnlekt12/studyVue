# **<<참고 노트>>** ([링크](https://clever-chandrasekhar-3500e1.netlify.app "블로그 바로가기"))
***

<br>
<br>


# ◎ 개요
```plaintext
1. 목표
    - 본 깃허브&블로그 개발에 대한 설명과 공부 과정을 다루는 항목.
2. 설명
    - 전체적인 소스에 대한 간략한 설명과 적용되어있는 내용을 다루는 항목.
3. 특정 항목 세부 설명
    - 평소 알던 내용이 아닌 한 번쯤은 되짚어 볼만한 있는 항목을 다루는 항목.
4. 참고 사이트&출처
    - 해당 블로그 & 깃허브 운영에 있어 도움이 된 사이트 & 출처를 다루는 항목.
```
***
<br>
<br>

## 1. 목표
> 프론트엔드 & 백엔드 공부 과정에서 배우게 되는 모든 과정에 대해서 기록하는 것이 목적.  
> 해당 마크다운 파일은 지속적으로 추가 수정될 예정.  

> 본 자료는 모두 상업적인 용도가 아닌 공부 목적이므로 참고가 될 만한 사항이 있다면 참고해도 무방함.  


***

<br>
<br>

## 2. 설명
우선 본인이 공부한, 그리고 앞으로 공부할 내용은 아래와 같다.  



순|주제|세부내용|비고  
:--:|:--:|:--:|--
1|프론트엔드 & 백엔드 기본|기본적인 이해 및 구분|
2|프론트엔드|HTML & CSS & JS기본|스타벅스 예제 사이트 제작
3|프론트엔드 프레임워크|각 분야별 개발 도구 설명 (사용법X)
4|GitHub|사용법|Netlify
5|JavaScript Essentials|사용법|Node.js
6|TypeScript Essentials|사용법
7|SCSS (CSS 전처리기)|사용법
8|Bundler|사용법|Redux, mobX, GraphQL, Next.js, Svelte
9|Vue.js|사용법|오프라인 강의 포함
10|React|사용법
11|백엔드|시작도 안함|패스트 캠퍼스 교육 이수 예정
***

<br>

## 3. 특정 항목 세부 설명
- 각종 기호 설명 (익숙치 않은 것만 다룸.)

  기호|영어|한글|비고
  :--:|:--:|:--:|--
  `|그레이브/백틱|?
  ~|틸드|물결
  @|앳(At sign)|골뱅이
  ^|캐럿||~ 이상을 의미
  "|쿼테이션|큰따옴표
  ()|퍼렌서시스|소괄호
  {}|브레이스|중괄호
  []|브래킷|대괄호
  <>|앵클브래킷|꺾새괄호

<br>

- 유용한 VSCode Extention List

  이름|설명|비고
  :--:|:--:|:--
  Korean|한글화|설치 후 명령 파레트에서 실행 가능 (cde)
  Beautify|코드 자동 정리|HookyQR.beautify 키워드 이용해 단축키 추가하여 자동 들여/내어쓰기 가능
  Auto Rename Tag|자동 태그|태그 열림/닫힘태그 자동 완성
  Live server|라이브 서버|브라우져 자동 열기 지원(테스트)

<br>

- 유용한 CDN List

  이름|설명|비고
  :--:|:--:|:--
  reset css|HTML 속성 초기화
  lodash|로-대쉬|쓰로틀(시간차 함수 실행)
  gsap|gsap|Js에서 HTML 요소 애니메이션 적용 (gsap.to)
  swiper|스와이퍼|슬라이드 기능

- Node Package List

  이름|설명|비고
  :--:|:--:|:--
  parcel-bundler(-D)|번들러|가상테스트:parcel index.html<br>빌드(번들):parcel build index.html
  lodash|데이터 관리 유틸리티
  typescript(-g)|js 컴파일러|npx tsc --init<br>tsc<br>tsc -w
  @popperjs/core|Popper
  bootstrap@next|디자인 Preset
  parcel-plugin-static-files-copy(-D)|정적파일 연결|"staticFiles":{<br>"staticPath":"static"<br>}
  postcss autoprefixer(-D)|브라우져 호환
  @babel/core @babel/preset-end(-D)|ES 컴파일러
  @vue/cli(-g)|vue 초기 구조 세팅
  vue-router@4|vue 컨트롤러
  @vuex@next|vue 상태관리패턴 구현도구
  axios|백엔드 API 호출 도구
  

<br>
<br>

***

## 4. 참고 사이트&출처
- **`패스트 캠퍼스`**  ( _[바로가기](http://fastcampus.co.kr)_ )  
    프론트 엔드 & 백엔드 전반적인 모든 교육 과정을 참고함.  

- **`평생 공부 블로그`**  ( _[바로가기](https://ansohxxn.github.io/blog/font/)_ )  
    참고할만한 내용이 많음.  
    웹 프로그래밍 외에도 유니티, 언리얼 등등에 대한 자료가 많음.
- **`Codepen.io`**  ( _[바로가기](https://codepen.io/)_ )  
    html 에 대해 간단한 프로그래밍 가능.
- **`Netlify`**  ( _[바로가기](https://www.netlify.com/)_ )  
    Github 의 특정 Repository 에 대해 도메인 없이 어플리케이션 개념으로 사이트를 구축하는 사이트.

- **`Easing-function`**  ( _[바로가기](https://developer.mozilla.org/en-US/docs/Web/CSS/easing-function)_ )  
    CSS에서 Transition 의 Timing-function 속성 지정시 참고할만한 사이트.


<!-- # vuetest

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/). -->
