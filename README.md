# NotoSansKR-Hestia-scss
----------

NotoSansKR-Hestia [GitHub Pages][1]를 참고해주세요.
 

차이점

- woff2 를 추가
- scss 추가
- font-weight 변경

| CSS Class       | weight 기존 | weight 변경 |
|-----------------|:----------:|:----------:|
| .noto-thin      |     100    |     100    |
| .noto-light     |   **300**  |   **200**  |
| .noto-demilight |   **350**  |   **300**  |
| .noto-regular   |     400    |     400    |
| .noto-medium    |     500    |     500    |
| .noto-bold      |     700    |     700    |
| .noto-black     |     900    |     900    |


## 수정법

### SCSS

* 폰트 경로 변경

`_variables.scss` 에서 `$noto-sans-path` 변경

```sass
$noto-sans-path: '/fonts' !default;
```

혹은 변수 미리선언 후 `@import`

```sass
$noto-sans-path: '/mydir/fonts' !default;
@import "NotoSansKR-Hestia";
```

* 컴파일 SCSS -> CSS

```bash
$ sass scss/NotoSansKR-Hestia.scss stylesheets/NotoSansKR-Hestia.css
```


## 사용법

### HTML
```html
<link href="/stylesheets/NotoSansKR-Hestia.css" rel="stylesheet" type="text/css">
```


### CSS
```css
@import url(/stylesheets/NotoSansKR-Hestia.css);
```


### CSS 헬퍼

#### .noto-sans
```
<span class="noto-sans">안녕하세요</span>
```

#### .noto-{weight}
```
<span class="noto-sans noto-demilight">안녕하세요</span>
```

[1]: http://theeluwin.github.io/NotoSansKR-Hestia
