# html-css-practice

## 텍스트 관련 태그

### 알고 있던 것

`<h`_n_`>` 태그들, `<p>` 태그, `<br>` 태그, `<b>` 태그, `<strong>` 태그, `<i>` 태그, `<span>` 태그

### 몰랐던 것

`<hr>` 태그, `<blockquote>` 태그와 `cite`속성, `<pre>` 태그와 이것이 웹 접근성에 문제가 될 수 있다는 점., `<em>` 태그, `<q>` 태그, `<mark>` 태그

---

## 리스트 태그

### 알고 있던 것

`<ul>` 태그, `<li>` 태그, `<ol>` 태그

### 몰랐던 것

`<ol>` 태그의 `type` 속성, `start` 속성, `<dl>`, `<dt>`, `<dd>` 태그

---

## 테이블 태그

### 알고 있던 것

`<table>` 태그, `<tr>`, `<th>`, `<td>` 태그, `border` 속성, `colspan`, `rowspan` 속성, `<thead>` 태그, `<tbody>` 태그

### 몰랐던 것

`<caption>` 태그, `<figure>` 태그, `<figcaption>` 태그, `aria-describedby` 속성, `<tfoot>` 태그, `<col>` 태그, `<colgroup>` 태그

---

## 이미지 태그

### 알고 있던 것

`<img>` 태그, `src` 속성, `alt` 속성, `width` 속성, `height` 속성

### 몰랐던 것

`<img>` 태그는 `<figure>` 태그의 대상이 될 수 있다. 즉, 단위가 되는 요소를 묶을 때 사용하는 것이 `<figure>` 태그다.

---

## 링크 태그

### 알고 있던 것

`<a>` 태그, `<a>` 태그의 `href` 속성, 앵커 태그

### 몰랐던 것

`<a>` 태그의 나머지 속성, 이미지 맵 태그(하나의 이미지에 여러개의 링크를 적용할 때 사용한다.)

---

## 폼 태그

### 알고 있던 것

`<form>` 태그와 `type` 속성, `method` 속성, `name` 속성, `action` 속성, `<label>` 태그, `<select>` 태그와 `<option>` 태그, `<button>` 태그

### 몰랐던 것

`target` 속성, `<fieldset>` 태그, `<legend>` 태그, 각종 type들의 사용법, `<optgroup>` 태그, `<datalist>` 태그, `<output>` 태그, `<progress>` 태그, `<meter>` 태그

---

# CSS

## CSS 주요 선택자

### 전체 선택자 - 모든 요소에 스타일 적용

주로 하위 요소에 한꺼번에 스타일을 적용할 때 사용하나, 전체 스타일을 초기화 할 때도 사용한다고 합니다.

### 태그 선택자 - 태그를 사용한 요소에 스타일 적용

전체 선택자 다음으로 많은 요소가 대상이 됩니다.

## Cascading Style Sheet

캐스캐이딩은 정말 중요한 개념 같아서 정리

CSS는 위에서 아래로 적용되고 다음의 규칙을 따른다.

1. 스타일 우선순위 - 스타일 규칙의 중요도, 적용 범위에 따라 우선순위가 결정되고 그 우선순위에 따라 위에서 아래로 스타일이 적용됩니다.
2. 스타일 상속 - 태그들의 포함관계에 따라 부모 요소의 스타일을 자식 요소로, 위에서 아래로 전달합니다.

### 스타일 우선순위

#### 얼마나 중요한가 - 중요도(Importance)

사(중) - 제(중) - 제(일) - 사(일) - 브

사용자 - 제작자: 사용자는 클라이언트 사용자가 사전에 정의, 제작자는 우리가 만드는 것

중요 - 일반: `!important`로 선언

브라우저

#### 얼마나 한정지을 수 있는가 - 명시도(Specificity)

스타일의 적용 범위에 따라 우선순위가 달라진다.

좁은 범위가 우선권을 가지고 넓은 범위가 가지지 못한다.

인라인 - id - 클래스 - 태그 - 전체

#### 소스에서의 순서(Source Order)

모두 같다면 소스에서 나중에 온 요소를 사용합니다.

### 스타일 상속

스타일 시트에서는 자식 요소에서 별도로 스타일을 지정하지 않으면 부모 요소에 있는 스타일 속성들이 자식 요소로 전달되는데 이를 '스타일 상속'이라고 합니다.

상속을 이용해서 효과적으로 스타일 시트를 만들 수 있습니다.

하지만, 모든 속성이 상속되지 않기 때문에 주의해야 합니다.
