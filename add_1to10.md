```
<p id="res">계산값</p>
<p class="c1">계산값</p>

<script>
    let sum = 0;
    for (let i = 1; i <= 10; i++) sum += i;
    const el1 = document.getElementById("res");
    el1.innerText = sum;

    const el2 = document.querySelector("#res");
    el1.innerText = sum;

    const el3 = document.getElementsByTagName("p")[0];
    el3.innerText = sum;

    const el4 = document.getElementsByClassName("c1")[0];
    el4.innerText = sum;
    el4.style.color="blue";
    console.log(sum);
</script>
```
