**문장을 클릭하면 글자 색이 초록색(green)에서 빨간색(red)으로 바뀌고**, 다시 클릭하면 원래대로 돌아오는 기능이에요.
---
#### 1. 이건 스타일(모양)을 정하는 부분이에요:

```html
<style>
    p {
        color: green;        /* 처음 글자 색을 초록색으로 */
        cursor: pointer;     /* 마우스를 올리면 손가락 모양으로 */
    }
</style>
```

#### 2. 이건 웹페이지에 보이는 글이에요:

```html
<p id="text">Click this line; green will change to red.</p>
```

- `<p>`는 문장을 나타내는 태그예요.
- `id="text"`는 이 문장을 JavaScript에서 찾아서 사용할 수 있도록 이름을 붙여준 거예요.

#### 3. 이건 동작(기능)을 정하는 JavaScript 코드예요:

```html
<script>
    const t = document.getElementById('text');  // id가 'text'인 문장을 가져옴

    t.onclick = () => {
        // 클릭했을 때 실행되는 함수
        // 지금 글자색이 'green'이면 'red'로 바꾸고,
        // 아니면 다시 'green'으로 바꿔요.
        t.style.color = t.style.color === 'green' ? 'red' : 'green';
    };
</script>
```

---

### 🧠 이 부분이 좀 어려울 수 있어요:

```javascript
t.style.color === 'green' ? 'red' : 'green';
```

이건 이렇게 생각하면 돼요:

- "지금 글자 색이 초록이면 빨간색으로 바꾸고,
- 아니면 초록색으로 바꿔!"

쉽게 풀어 쓴 코드로 바꾸면:

```javascript
if (t.style.color === 'green') {
    t.style.color = 'red';
} else {
    t.style.color = 'green';
}
```

---
### 위 코드를 실행하고 테스트 할때 문제점 2가지를 찾아보세요.
1. 문제1:
2. 문제2:

## 문제가 해결된 코드
---

```
<style>
    p {
        color: green;
        cursor: pointer;
        user-select: none; /* ✅ 텍스트 선택 방지 */
    }
</style>

<p id="text">Click this line; green will change to red.</p>

<script>
    const t = document.getElementById('text');
    t.style.color = 'green'; /* ✅ 처음으로 초록색 선택 */
    t.onclick = () => {
          t.style.color = t.style.color === 'green' ? 'red': 'green';
    };
</script>
```
