---
title: "⛏️ 불 크기가 1바이트인 이유"
date: 2023-03-16. 10:51
last_modified_at: 2023-03-16. 10:51
categories: ⛏️Memo
---

0과 1, 두 개의 상태만을 가지기에,  
1비트만 가지면 될 것 같은 불(Boolean)이,  
1바이트나 용량을 가지는 이유는,  

현대 컴퓨터 구조 상,  
비트 단위로 데이터에 접근하지 않고,  
바이트 단위로 주소/데이터에 접근하기 때문  

일반적으로 CPU의 구현에 따른 최소 단위로 크기가 설정된다  

[참고 - 스택오버플로우](https://stackoverflow.com/questions/2064550/)  
[참고 - 1바이트는 왜 8 비트인가](https://zepeh.tistory.com/313)  
