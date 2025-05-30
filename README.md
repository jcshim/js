
### ✅ JavaScript란? (정의)

> **JavaScript는 웹 페이지를 살아 움직이게 만드는 언어예요.**

HTML은 뼈대,  
CSS는 꾸미는 옷,  
JavaScript는 움직임과 행동을 담당해요.

예를 들어,
- 버튼을 누르면 창이 뜨고,
- 글자가 바뀌고,
- 스크롤하면 애니메이션이 생기고...

이런 걸 **JavaScript**가 해줘요!

---

### ✅ JavaScript를 어떻게 배우면 좋을까? (정말 쉬운 방법)

#### 1. **기본 문법부터 살짝 맛보기**
- 변수: `let name = "홍길동";`
- 조건문: `if (score > 90) { ... }`
- 반복문: `for (let i = 0; i < 5; i++) { ... }`
- 함수: `function sayHello() { alert("안녕!"); }`

👉 이런 문법을 통해 컴퓨터에게 "무엇을 어떻게 해!"라고 말하는 방법을 배우는 거예요.

---

#### 2. **웹 브라우저에서 바로 실습하기**
아무 웹 페이지에서 **F12** 누르고 → **콘솔(Console)** 탭에 아래처럼 입력해 보세요:

```javascript
alert("안녕, 자바스크립트!");
```

👉 바로 팝업 창이 뜰 거예요! 놀랍죠?

---

#### 3. **작은 프로젝트 해보기**
예를 들면…
- 버튼 클릭하면 글자가 바뀌는 웹페이지 만들기
- 간단한 계산기 만들기
- 랜덤 숫자 맞추기 게임 만들기

👉 직접 만드는 게 최고의 공부예요!

---

#### 4. **추천 학습 루트**
- **기초 튜토리얼**: [https://ko.javascript.info](https://ko.javascript.info)
- **유튜브 강의**: "자바스크립트 기초"로 검색
- **코딩 실습 사이트**: [https://codepen.io](https://codepen.io), [https://replit.com](https://replit.com)


## 또다른 예제, F12 누르고
```
const box = document.createElement("div");
box.innerHTML = `<me style="font-size:24px; cursor:pointer; color:blue;">국립경국대학교</me>`;
box.style = "position:fixed;top:20px;left:20px;background:#f0f0f0;padding:20px;border:1px solid #ccc;border-radius:8px";
document.body.appendChild(box);
box.querySelector("me").onclick = () => window.open("https://www.gknu.ac.kr", "_blank");
```
