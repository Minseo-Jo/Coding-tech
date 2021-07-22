# CSS
-------------------------------------------------------------
```
Cascading Style Sheets
HTML이 정보를 표현한다면
CSS는 HTML을 시각적으로 꾸며주는 역할을 한다. 
```

### HTML에서 CSS 사용하기
---------------------------------------
- Inline
  - Element에 스타일을 직접 기술하는 방식
  - 셀렉트가 필요 없다.
  - CSS 선언이 분명해서 style tag 방식에 비해 엘리먼트에 영향을 주고 있는 CSS를 추적하기가 쉽다.
  - 코드가 많아지고, 의미와 디자인의 분리라는 CSS의 취지와 벗어난다.

- [Internal][link] 
  - style 태그에 기술하는 방식
  - inline 방식 대비 경제적으로 코딩할 수 있다.
  - 의미와 디자인의 분리라는 CSS의 취지에 부합한다.

- [External][link2] 
  - CSS를 별도의 파일로 분리해서 링크하는 방식
  - 문법적으로는 style tag와 동일
  - 파일의 교체로 디자인을 변경할 수 있다는 점에서 유지보수가 편리하다.

[link]: https://github.com/Minseo-Jo/Coding-tech/blob/e817950f15caefd9c7f3bd30793e0f2f2c73a424/Web/CSS/javaScriptTesting_css.html
[link2]: https://github.com/Minseo-Jo/Coding-tech/blob/e817950f15caefd9c7f3bd30793e0f2f2c73a424/Web/CSS/basic.css


### CSS Syntax
----------------------------------------------------------

<img src=http://www.w3schools.com/css/selector.gif></img>


### CSS Selector
---------------------------------------------------------------
> CSS의 효과가 적용될 태그를 지정

- Element selector
  - 특정 태그명을 가진 엘리먼트 전체를 제어하기 위해서 사용
  - css선택자에서는 태그의 이름을 사용함


  Example)
  ```css
  p {
    color: red;
    text-align: center;
  }
  ```

- ID selector
  - id 속성은 전체 문서에서 하나의 태그를 식별하기 위해서만 사용됨
  - 우선순위가 가장 높음
  - css 선택자에서는 #을 사용해서 id임을 표시

  Example)
  ```css
  #para1 {
    text-align: center;
    color: red;
  }


- Class selector
  - class 속성은 일련의 태그를 그룹핑해서 하나처럼 제어하기 위해서 사용
  - class 속성에는 공백으로 구분된 여러개의 class가 표시될 수 있음
  - css선택자에서는 '.'을 사용해서 class임을 표시

  Example)
  ```css
  .center {
    text-align: center;
    color: red;
   }
