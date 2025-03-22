```
<style>p { color: blue;  cursor: pointer;}</style>
<p id="text">안녕하세요!</p>
<script>
  const text = document.getElementById('text');
  text.onclick = () => {
    text.style.color = (text.style.color === 'red') ? 'blue' : 'red';
  };
</script>
```

이 코드는 HTML, CSS, JavaScript를 사용해서 간단한 텍스트 색상 변경 기능을 구현한 예제야. 쉽게 설명해 줄게.

### HTML
```html
안녕하세요!
```
- **``**: 문단을 나타내는 태그.
- **`id="text"`**: 이 문단을 JavaScript에서 쉽게 참조할 수 있도록 고유한 식별자로 설정.

### CSS
```css

  p {
    color: blue; /* 기본 색상은 파란색 */
    cursor: pointer; /* 마우스를 올리면 손가락 모양으로 바뀜 */
  }

```
- **`color: blue`**: 문단의 기본 색상을 파란색으로 설정.
- **`cursor: pointer`**: 마우스를 문단 위에 올리면 손가락 모양으로 바뀌어서 클릭할 수 있는 요소임을 시각적으로 나타냄.

### JavaScript
```javascript

  const text = document.getElementById('text'); // HTML의  요소를 가져옴
  text.onclick = () => {
    // 클릭할 때마다 색상을 파란색과 빨간색으로 번갈아 바꿈
    text.style.color = (text.style.color === 'red') ? 'blue' : 'red';
  };

```
- **`document.getElementById('text')`**: HTML에서 `id="text"`로 설정된 요소를 가져옴.
- **`text.onclick`**: 이 요소가 클릭될 때 실행할 함수를 설정.
- **`text.style.color`**: 요소의 색상을 변경. 현재 색상이 빨간색이면 파란색으로, 아니면 빨간색으로 바꿈.

이 코드를 실행하면, "안녕하세요!"라는 문장을 클릭할 때마다 색상이 파란색과 빨간색으로 번갈아 변하는 것을 볼 수 있어.
