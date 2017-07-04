# 기초반 HTML, CSS 박스 레이아웃

'HTML' 과 'CSS' 를 이용하여 레이아웃을 연습하세요.

## View Site

### [레이아웃1-1](http://herop.me/layouts/layout-1-1)

`margin: 0 auto` 를 사용하여 **중앙 정렬**.  
`width` 속성 필수!

```css
width: 300px;
margin: 0 auto;
```

### [레이아웃1-2](http://herop.me/layouts/layout-1-2)

`float: left` 로 수평 정렬하고 중간 여백을 줄 경우,  
`:last-child` 를 사용하여 마지막 요소(element)의 우측 **여백(margin) 제거**.

```css
.container li {
    margin-right: 10px;
}
.container li:last-child {
    margin-right: 0;
}
```
  
### [레이아웃2-1](http://herop.me/layouts/layout-2-1)

`.inner` 를 사용하여 섹션 콘텐츠의 **중앙 정렬**.

```html
<div class="inner"></div>
```
  
### [레이아웃2-2](http://herop.me/layouts/layout-2-2)

`inner` 요소 내부에 콘텐츠 추가하기
  
### [레이아웃2-3](http://herop.me/layouts/layout-2-3)

`float: left` 와 `float: right` 를 동시 사용하여 요소들을 **양쪽으로 정렬**.

```css
.logo {
    float: left;
}
.menu {
    float: right;
}
```

`float`의 값이 존재하는 요소에서는 '마진 병합' 현상이 발생하지 않습니다.

```css
.logo {
    margin-top: 15px;
    float: left;
}
.menu {
    margin-top: 20px;
    float: right;
}
```
  
### [레이아웃3-1 (iRiver)](http://herop.me/layouts/layout-3-1)

'iRiver' 페이지(UI) 레이아웃 연습.

'Logo, Sub, Main' 의 각 기능을 분리하고 Markup 하는 순서(HTML 계층구조)를 정리하세요.

```html
<ul class="sub_menu"></ul>

<div class="logo"></div>

<ul class="main_menu"></ul>
```

`float` 속성을 사용 후 바로 `clearfix` **해제**하세요.

```html
<ul class="sub_menu clearfix"></ul>
```

`inner` 요소 내부에 콘텐츠를 추가하여 **중앙 정렬**하세요.

```html
<div class="inner"></div>
```

`float` 으로 **정렬**하고 `position` 으로 **배치**하세요.

```css
.quick_menu li {
    float: left;
    margin-right: 25px;
}

.family_site {
    position: absolute;
    top: 15px;
    right: 0;
}
```
