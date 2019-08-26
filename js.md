## js編(v8)

---

js engine
- chrome v8
- firefox spider monkey
- safari javascript core
- edge chakra core => v8

---

### JIT
Just-In-Time Compiler

---

![](https://miro.medium.com/max/2038/1*ZIH_wjqDfZn6NRKsDi9mvA.png)
- method JIT

コンパイルの単位はfunction ごとに行われる

頻繁に呼ばれる関数と短い関数が最適化される。

---

### hidden class | shape

```javascript 1.8
const o1 = {};
o1.x = 3;
o1.y = 4;

const o2 = {};
o2.x = 5;
o2.y = 6;
```

|||

<img style="height: 80vh;background: #fff;" src="https://camo.githubusercontent.com/546a04fe2b673df407a6fe5ae96fc6f2fd75b903/68747470733a2f2f696d616765732e706f6e79666f6f2e636f6d2f75706c6f6164732f372d38366535353433623430383934613137383734326161613934636130643761322e737667">

|||

![](https://images.ponyfoo.com/uploads/1-8b65bb067a394418bd9858de58bad17a.svg)

Smi = small integer 31bit の符号付整数

---

### gc

optimization killer
