# HTML
> HTML(HyperText Markup Language)는 웹 페이지를 기술하기 위한 마크업 언어이다.  
> 내용(content)과 구조(structure)를 담당하며 태그를 통해 정보를 구조화한다.

## 기본 구조
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Hello World</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>안녕하세요! HTML5</p>
  </body>
</html>
```
- `<head>`태그 사이에는 document title, 외부 파일의 참조, 메타데이터의 설정 등이 위치하며 이 정보들은 브라우저에 표시되지 않는다.
- 웹 페이지에 출력되는 모든 요소는 `<body>`태그 사이에 위치한다.

## 기본 문법

### 요소 (Element)
HTML 요소는 시작 태그(start tag)와 종료 태그(end tag) 그리고 태그 사이에 위치한 content로 구성된다.
```html
<p>Hello</p>

<p>   : 시작태그
Hello : 콘텐츠
</p>  : 종료태그
```
HTML문서는 요소(Element)들의 집합으로 이루어진다.

다양한 태그가 존재하며 이를 적절하고 문법에 맞게 작성하면 검색엔진이 웹 페이지를 더 잘 인식하고 색인화 하는데에 도움을 주어 검색 엔진 최적화에 도움을 준다.

[HTML 태그 참고서(요소 참고서)](https://developer.mozilla.org/ko/docs/Web/HTML/Element)

### 어트리뷰트(Attribute)
어트리뷰트란 요소의 성질, 특징을 정의하는 명세이다. 요소의 추가적 정보를 제공한다.  
어트리뷰트는 시작 태그에 위치해야 하며 이름과 값의 쌍을 이룬다.
```html
<img src="html.png">

src        : 어트리뷰트명
"html.png" : 어트리뷰트값
```

