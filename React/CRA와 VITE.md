# CRA? VITE?
>CRA(Create React App) facebook에서 제공하는 React 어플리케이션을 쉽고 간편하게 생성할 수 있는 도구이다.

>Vite는 원래 `vue.js` 개발을 위한 도구로 `vue.js`어플리케이션 개발에 최적화 되어 있지만, 다른 프레임워크나 라이브러리에서도 사용이 가능하다.


## CRA(Create React App)
CRA는 리액트 팀이 추천하는 공식 리액트 보일러 플레이트로 초기 설정의 간편함과 Webpack, Babel, ESLint 등 다른 복잡한 툴을 몰라도 개발을 시작할 수 있어 많은 사용자 사용하는 도구이다.

### 시작하기
```bash
npx create-react-app 프로젝트명
```
※ npx를 사용하는 이유는 버전 변경이 자주 있으며 글로벌 환경에서 관리해주기 위해 npx를 이용하여 최신버전을 실행하는 것을 권장한다.

### 장점
- Webpack, Babel, ESLint 등 모둘 번듈러, 트랜스파일러를 자동으로 설정해줘 초보자가 접근하기 쉽다.
- ES6+문법, CSS 후처리와 같은 개발환경을 자동으로 설정해준다.

### 단점
- Webpack, Babel 의 설정을 변경하기 어렵다. (eject 사용해서 수정해야한다.)
- 높은 추상화로 설정 flow를 알기 힘들다.
- SSR이나 CSR을 위해 별도의 작업이 필요하다.

## Vite
Vite는 Esbuild를 기반으로 만들어진 빠르고 간결한 모던 웹 프로젝트 개발 경험에 초점을 맞춰 탄생한 빌드 도구이다.

>지원중인 템플릿
> - vanilla
> - vue
> - react
> - preact
> - lit
> - svelte

### 시작하기

**Vite 설치**
```
npm create vite@latest

yarn create vite
```
**템플릿 설치**
```bash
# npm 6.x
npm create vite@latest ${디렉터리 명} --template ${템플릿 명}

# npm 7+
npm create vite@latest ${디렉터리 명} -- --template ${템플릿 명}

# JavaScript react 템플릿 생성
npm create vite@latest vite-test -- --template react

# TypeScript react-ts 템플릿 생성
npm create vite@latest vite-test -- --template react-ts
```

### 장점
- ESM 방식을 사용하기 때문에 로컬 서버 구동 속도가 매우 빠르다.
- HMR을 기본적으로 지원하며, 애플리케이션의 변경 사항이 실시간으로 반영된다.
- 타입스크립트를 기본적으로 지원하며, 타입 검사와 같은 기능을 더욱 쉽게 사용할 수 있다.

### 단점
- 기존에 웹팩을 사용하던 프로젝트에서 마이그레이션 진행할 때 불편하다.

## 결론
처음 React를 배울때에는 프로젝트 생성하는 방법이 CRA만 존재하는 줄 알았다. 그 시기에는 Webpack, Babel 등 번들러에 대한 이해가 부족했기 때문이다.

React를 통해 여러 프로젝트를 만들어보고 계속 공부를 진행하면서 번들러에 대한 이해가 조금 올라가고 다양한 빌드 도구들을 알아가면서 CRA 말고 다른 빌드 도구를 사용해보고 싶어졌기 때문에 해당 내용을 정리해 보았다.

