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
