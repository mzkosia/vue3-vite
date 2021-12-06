1. vue3 기초

cdn
npm/yarn

2. cdn을 통한 hello world 구현

3. npm/vite를 이용한 기본 프로젝트 생성

lazy 로딩 방식

    npm install vue@next

    npm init @vitejs/app hello-world-vite2

    npm install (yarn install)

    npm run dev

    npm run build

vite 기본 프로젝트 구성
index.html
app (id 값)
main.js
index.css
template / script setup(props / defineProps / reactive)  / style(scoped)

vite alias 생성

    npm install path

root 폴더 vite.config.js

독립형 Vue-devtools 연동

    vue-devtools

index.html head 태그 마지막 

\<script src="http://localhost:8098"></script>\ 

    npm run dev

4. vue 3 핵심 문법

single file compnent(sfc) - template / script / style

컴포지션 함수 setup - options API -> 컴포지션 API(data / methods / computeed 정의 필요 없음)

vue 컴포넌트의 생명주기 - 생명주기 후킹(hook) 차이
참조(../image/vue-생명주기...)(../image/vue-3-생명주기)(https://hyeooona825.tistory.com/40)

선언적 렌더링 - 수염표기법 객체형식 반환 (es6 단축속성)
v-text 디렉티브

v-html 디렉티브를 이용한 html 표현(v-text와 차이)
v-pre 디렉티브를 이용한 컴파일 무시
데이터 결합을 통한 사용자 입력처리(v-bind, v-model, ref, 템플릿 변경)

v-model 디렉티브 수식어(수식어보단 내부 구현, 사용자 수식어를 통해 처리)

이벤트 리스너를 이용한 사용자 입력 처리(v-on, @)

이벤트 수식어 / 키수식어
(https://kr.vuejs.org/v2/guide/events.html - 이벤트 / 키 수식어)

템플릿 내 조건문(v-if(else-if) / v-show )

템플릿 내 반복문(v-for(in)-reactive-배열 객체 키 )

computed 속성

watch와 watchEffect(차이점) ????

컴포넌트 생성 (application API)(https://v3.ko.vuejs.org/api/application-api.html#component)

props(https://v3.ko.vuejs.org/guide/component-props.html#prop-%E1%84%90%E1%85%A1%E1%84%8B%E1%85%B5%E1%86%B8)

non-props 속성 - $attrs ???

사용자 이벤트 생성 - emits (케밥형식의 소문자)

v-model 디렉티브와 이벤트 결합

slots(데이터 전달 - slot props를 이용한 데이터 결합)

provide  / inject (vue2의 event bus)

사용자 디렉티브 - directive 함수, 바인딩 객체 속성 ???

mixins (컴포넌트보다 먼저 호출된다)(vue 3에서는 컴포지션 API 권장) ???

실전 예제를 통한 문법 복습

- 사용자 입력 처리 ( ../practive/3/1. inputs)
- 사용자 정의 버튼 ( ../practive/3/2. custom_button)(props와 css 연결)
- 사용자 정의 table ( ../practive/3/2. custom_table)
