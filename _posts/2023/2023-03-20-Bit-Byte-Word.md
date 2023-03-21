---
title: "⛏️ Bit Byte KiloByte Word"
date: 2023-03-20. 16:53
last_modified_at: 2023-03-20. 16:53
categories: ⛏️Memo
---

[참고 0](https://en.wikipedia.org/wiki/Byte)  
[참고 1](https://velog.io/@victor/1kb-1024-bytes-1000-bytes-%EB%AD%90%EA%B0%80-%EB%A7%9E%EC%9D%84%EA%B9%8C-mojurs3pb2)  
[참고 2](https://ko.wikipedia.org/wiki/X86)  
[참고 3](https://eine.tistory.com/entry/64%EB%B9%84%ED%8A%B8-32%EB%B9%84%ED%8A%B8-CPU%EC%99%80-%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C-%EC%97%90-%EB%8C%80%ED%95%98%EC%97%AC)  
[참고 4](https://softwareengineering.stackexchange.com/questions/120126/what-is-the-history-of-why-bytes-are-eight-bits)  
[참고 5 - WORD](https://bebesoft.tistory.com/12?category=887595)  

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

---

32-Bit, 64-Bit  

Program Counter  
32-Bit = 2^32 = 4,294,967,296  
64-Bit = 2^64 = 18,446,744,073,709,551,616  
32-Bit = 약 4-GB 메모리  
64-Bit = 약 256-TB 메모리 (48-Bit만 사용)  

왜 48-Bit만 사용?  
'일반적으로', 256-TB 이상의 주소 공간을 사용하지 않음  

운영체제도 32-Bit, 64-Bit 로 나뉨  
32-Bit CPU 에는 64-Bit 운영체제가 동작하지 않음 .  
64-Bit CPU 에는 32-Bit 운영체제가 동작하기는 하지만 하위 호환 Backward Compatibility 됨.  

앱 역시 32-Bit, 64-Bit 로 나뉨  
32-Bit 운영체제에는 64-Bit 앱이 동작하지 않음 .  
64-Bit 운영체제에는 32-Bit 앱이 동작하기는 하지만 하위 호환 Backward Compatibility 됨.  

---

x86, x64 (x86-64)  

x85 = 8-bit  
x86 = 32-Bit (일반적으로)  
x64 = 64-Bit (x86-64)  

x86 (80x86) =  
1978년 인텔이 개발한 인텔 8086에 적용된 아키텍쳐,  
그 호환 프로세서와 후속작 (8086의 명령어 세트를 기반하여 확장한, 386, 486, ...  )  

IA-16, IA-32, IA-64 를 모두 포함하는 단어이지만,  
일반적으로 x86이라 하면 IA-32을 지칭  

IA Intel Architecture

---

워드 WORD  
기계어 명령어나 연산을 통해 저장된 장치로부터 레지스터에 옮겨 놓을 수 있는 데이터 단위  
= CPU가 처리할 수 있는, 버스에 한 번에 지나갈 수 있는 크기의 단위  
= DTU Data Transport Unit (DTU를 사용하는 용어가 많았기에 WORD로)  

컴퓨터 아키텍쳐에서  
32-Bit = WORD : 32-Bit  
64-Bit = WORD : 64-Bit  

프로그래밍에서  
Win32 API의 WORD = 16-Bit  
왜 와이  

IA-16 기본 처리 단위 DTU = WORD = 16-Bit  
추후 32-Bit, 64-Bit 등의 프로세서 (IA-32, IA-64 등) 등장  

호환성의 문제으로 인해, 기존 단위 크기를 바꿀 수는 없고,  
때문에 기존 16-Bit Word를 기반으로 한 새로운 단위  
DWORD = Double Word = 32-Bit  
QWORD = Quad/Quotable Word = 64-Bit  


---

컴퓨터에서의 1K = 1024  
I.E. 1 KB = 1024 Byte  
왜 와이  

k, Kilo, 10^3, SI 접두어  
1 KM, 1 KG 등 여러 단위에 쓰이는 킬로  

컴퓨터에서도 큰 단위를 다룰 때 킬로를 사용하는데,  
2진수를 사용하는 컴퓨터 시스템에서 1000은 다루기 복잡한 숫자  
1000 = b1111101000  

때문에 2진수 컴퓨터 시스템에서 다루기 쉽도록 2의 배수이면서,  
가장 원래 1K = 1000 에 가까운, 2^10 = 1024를 컴퓨터 시스템에서의 1K로 사용  
1024 = b10000000000  

기억장치를 팔 때에는,  
기존 1K = 1000 단위로 광고하여 팔기 때문에,  
500GB 부품을 사도 컴퓨터는 466GB로 인식  

인터넷 속도도 비슷한 이유로,  
MB가 아닌 Mb로 팔기 때문에,  
100Mb 서비스를 사도 12.5MB로 인식  

