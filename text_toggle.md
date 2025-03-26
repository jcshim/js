## Click this line; green will change to red.

```
<style>
    p {
        color: green;
        cursor: pointer;
    }
</style>

<p id="text">Click this line; green will change to red.</p>

<script>
    const t = document.getElementById('text');
    t.onclick = () => {
          t.style.color = t.style.color === 'green' ? 'red': 'green';
    };
</script>
```
### 이 코드를 실행하고 테스트 할때 문제점 2가지를 찾아보세요.
1. 문제1:
2. 문제2:

## 문제가 해결된 코드

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
