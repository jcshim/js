### 📝 기능
- 할 일 입력 후 "추가" 버튼 클릭 시 목록에 추가
- 항목 클릭 시 "완료" 표시 (취소선)
- 삭제 버튼으로 항목 삭제

---

### ✅ 전체 코드

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <title>To-Do List</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
            background-color: #f0f0f0;
        }
        h1 {
            color: #333;
        }
        input[type="text"] {
            padding: 10px;
            width: 200px;
            font-size: 16px;
        }
        button {
            padding: 10px 15px;
            font-size: 16px;
            margin-left: 5px;
            cursor: pointer;
        }
        ul {
            list-style: none;
            padding: 0;
            margin-top: 20px;
        }
        li {
            background-color: #fff;
            margin: 10px auto;
            padding: 10px 15px;
            width: 300px;
            border-radius: 5px;
            text-align: left;
            position: relative;
        }
        li.completed {
            text-decoration: line-through;
            color: gray;
        }
        .delete-btn {
            position: absolute;
            right: 10px;
            top: 10px;
            background: red;
            color: white;
            border: none;
            border-radius: 3px;
            cursor: pointer;
            padding: 3px 7px;
        }
    </style>
</head>
<body>

    <h1>나의 할 일 목록</h1>
    <input type="text" id="todo-input" placeholder="할 일을 입력하세요">
    <button onclick="addTodo()">추가</button>

    <ul id="todo-list"></ul>

    <script>
        function addTodo() {
            const input = document.getElementById("todo-input");
            const text = input.value.trim();
            if (text === "") return;

            const li = document.createElement("li");
            li.textContent = text;

            // 완료 표시 toggle
            li.addEventListener("click", () => {
                li.classList.toggle("completed");
            });

            // 삭제 버튼
            const deleteBtn = document.createElement("button");
            deleteBtn.textContent = "삭제";
            deleteBtn.className = "delete-btn";
            deleteBtn.onclick = (e) => {
                e.stopPropagation(); // 부모 li 클릭 방지
                li.remove();
            };

            li.appendChild(deleteBtn);
            document.getElementById("todo-list").appendChild(li);
            input.value = "";
        }
    </script>

</body>
</html>
```

---

### 💡 사용법
1. HTML 파일로 저장 (예: `todo.html`)
2. 더블 클릭해서 브라우저에서 열기
3. 할 일을 입력하고 "추가" 버튼 클릭!
