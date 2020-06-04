# Reminder

목차

1. [프론트엔드 개발 환경 셋업하기](##프론트엔드-개발-환경-셋업하기)
2. [자바스크립트 문법](##자바스크립트-문법)
3. [Git 협업 과정](##Git-협업-과정)

## 프론트엔드 개발 환경 셋업하기

<details>
  <summary>
    왜 Node.js를 사용하는가?
  </summary>
  <ul><ul>
    <li>
    좋은 자바스크립트 실행 환경이기 때문이다. 싱글 스레드 기반 특성 때문에 블로킹 이슈가 심각해지자 비동기 - 이벤트 주도 아이디어를 통해 블로킹 시간을 최소화하는 목적으로 설계됐다.
    </li>
  </ul></ul>
 </details>

<details>
  <summary>
    왜 npm을 사용하는가?
  </summary>
  <ul><ul>
    <li>
    남들이 작업해놓은 유용한 패키지를 가져다 쓰기 쉽게 도와준다. 의존성 관리를 통해 환경 차이에서 발생하는 문제들을 경감시켜 준다.
    </li>
  </ul></ul>
 </details>

 <details>
  <summary>
    왜 webpack을 사용하는가?
  </summary>
  <ul><ul>
    <li>
    첫번째, 자바스크립트 변수 유효 범위 이슈를 ES6 modules 문법과 웹팩의 번들링으로 해결해준다. 두번째, 파일의 압축과 병합으로 총 HTTP 요청 횟수를 줄여 성능을 높여준다. 세번째, 원하는 모듈을 원하는 시점에 로딩하여 성능을 높여준다.
    </li>
  </ul></ul>
 </details>

 <details>
  <summary>
    왜 ESLinter를 사용하는가?
  </summary>
  <ul><ul>
    <li>
    코드 품질을 관리해준다. 개발자가 실수하기 쉬운 부분들을 점검하여 알려준다. 치명적인 실수를 줄여주고 보기 좋은 코드를 만들도록 돕는다.
    </li>
  </ul></ul>
 </details>

 <details>
  <summary>
    왜 Barbel을 사용하는가?
  </summary>
  <ul><ul>
    <li>
    브라우저마다 사용되는 언어가 조금씩 다른데, 모든 브라우저에서 호환되는 코드로 트랜스파일하여 잘 작동되게 하기 위해서다.
    </li>
  </ul></ul>
 </details>

<details>
  <summary>
    왜 JSX를 사용하는가?
  </summary>
  <ul><ul>
    <li>
    자바스크립트를 사용하여 최종적인 UI를 만들고 조작하기 편하기 때문이다. 즉 자바스크립트로 HTML 문서를 편하게 만들고 조작할 수 있다.
    </li>
  </ul></ul>
 </details>

## 자바스크립트 문법

* [Object](https://ko.javascript.info/object)
* [Array](https://ko.javascript.info/array)
* [Rest Parameter](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Functions/rest_parameters)
* [Spread Syntax](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Spread_syntax)
* [Destructuring Assignmnet](https://ko.javascript.info/destructuring-assignment)
* [Object.entries()](https://ko.javascript.info/keys-values-entries)
* [||](https://ko.javascript.info/logical-operators#ref-327)

## Git 협업 과정
1. 프로젝트 init 또는 clone
2. origin, upstream 세팅 확인
3. 작업 브랜치 생성
4. 작업
5. [commit](https://djkeh.github.io/articles/How-to-write-a-git-commit-message-kor/)
6. origin push
7. Pull Request
8. 수정 또는 완료