---
title: "⛏️ Bit Byte Word"
date: 2023-03-20. 16:53
last_modified_at: 2023-03-20. 16:53
categories: ⛏️Memo
---

Byte = 8 Bit  
왜 와이  

본래 Byte는 컴퓨터에서 문자 하나를 표현하기 위한 비트 수  
이가 확장되어, '디지털 정보의 가장 작은 단위'  

과거엔 바이트의 크기가 하드웨어에 종속되었고, 명확한 표준이 없었음  
곳에 따라 1 ~ 48 Bit 범위의 크기로 사용되었었다고 함  

6 Bit를 사용하는 문자 표현 방식이 주로 사용되었고,  
1960년대에는 6 Bit, 9 Bit 를 사용하는 컴퓨터가 일반적이었다고 함.  
이런 컴퓨터들은 2, 3, 4, 5, 6, 8, 10 6-Bit Byte에 상응하는, 12, 18, 24, 30, 36, 48, 60 Bit의 Memory Word를 주로 사용했음.  
이 시대엔 이런 Bit Groupings를 Syllables, Slab 등으로 불렀음. (Byte가 일반화되기 전까지)  

현대의 사실상 표준 De Facto Standard 이 된 8-Bit Byte는,  
ISO/IEC 2382-1:1933 에 문서화 되었음.  

ISO International Organization for Standardization  
IEC International Electrotechnical Organization  

ASCII Code는 7 Bit 만으로도 필요로 하는 문자를 모두 표현 할 수 있었는데,  
2진수를 사용하는 컴퓨터 구조 특성상, 편리하게 2의 배수로 만들기 위해,  
7 Bit 에 1 Bit 를 더하여 8 Bit로 만들어 사용  

이가 널리 쓰이면서 사실상 표준이 됨.  

현대 컴퓨터 Architecture 도 이를 기반으로 8의 배수인 32-Bit, 64-Bit Words 를 사용하게 됨.  