웹 개발에서 `style`은 웹 페이지의 디자인과 레이아웃을 조정하는 **CSS(Cascading Style Sheets)**를 의미

---

## 🌱 CSS 기초 학습 자료

### 1. **CSS란 무엇인가?**
- HTML로 만든 웹 페이지에 **색상, 폰트, 배치** 등을 입히는 도구
- HTML은 구조, CSS는 스타일을 담당

---

### 2. **기초 문법**
```css
선택자 {
    속성: 값;
}
```
예:
```css
p {
    color: blue;
    font-size: 16px;
}
```

---

### 3. **자주 쓰는 CSS 속성**

| 속성        | 설명                           | 예시 값               |
|-------------|--------------------------------|------------------------|
| `color`     | 글자 색                        | `red`, `#333`, `rgb(0,0,0)` |
| `background-color` | 배경색             | `lightgray`            |
| `font-size` | 글자 크기                      | `14px`, `1.2em`        |
| `margin`    | 바깥 여백                      | `10px`, `0 auto`       |
| `padding`   | 안쪽 여백                      | `5px`, `1em`           |
| `border`    | 테두리                         | `1px solid black`      |
| `text-align`| 글자 정렬                      | `left`, `center`       |
| `display`   | 요소의 레이아웃 방식 설정      | `block`, `inline`, `flex` |

---

### 4. **선택자 종류**
```css
/* 전체 선택자 */
* { margin: 0; padding: 0; }

/* 태그 선택자 */
p { color: green; }

/* 클래스 선택자 */
.box { background: yellow; }

/* 아이디 선택자 */
#title { font-weight: bold; }
```

---

### 5. **추천 온라인 학습 자료**

| 제목 | 설명 | 링크 |
|------|------|------|
| [MDN Web Docs - CSS](https://developer.mozilla.org/ko/docs/Web/CSS) | 가장 신뢰받는 공식 문서 | 🔗 [바로가기](https://developer.mozilla.org/ko/docs/Web/CSS) |
| [W3Schools - CSS Tutorial](https://www.w3schools.com/css/) | 인터랙티브 예제 중심 | 🔗 [바로가기](https://www.w3schools.com/css/) |
| [CSS Diner](https://flukeout.github.io/) | 선택자 연습 게임 | 🔗 [바로가기](https://flukeout.github.io/) |
| [Flexbox Froggy](https://flexboxfroggy.com/) | Flexbox 레이아웃 연습 게임 | 🔗 [바로가기](https://flexboxfroggy.com/) |

---
