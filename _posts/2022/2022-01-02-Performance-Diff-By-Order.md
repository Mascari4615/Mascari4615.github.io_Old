---
title: "⛏️ 연산 순서에 따른 퍼포먼스 차이"
date: 2022-01-02. 12:07
categories: ⛏️Programming 🕯️Programming-Memo
---
## 💎

---

![참고](\assets\img\0003.png)

연산 순서에 따라 퍼포먼스 차이가 발생한다  
당연한 말이긴 하지만  

VS 2022 에서 제안하는 것들 중 도움되는 것이 참 많은 것 같다.  

230109  
[Short-Circuit Evaluation](https://ttmdacl.github.io/posts/Short-Circuit-Evaluation/)  
Short-Circuit Evaluation 에 따른 연산 순서 상의 속도 차이도 존재한다.  
요약하면 비용이 높은 함수를 뒤쪽에 배치하면 좋다.  
