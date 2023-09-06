---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day2
---

<div class="flex h-full space-x-8  mb-14 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-60 block"> 與 JS & ECMAScript</span> 
  </div>
  <div class="h-42 w-42">
    <img src ="/tslogo.png" class="mx-auto"/>
  </div>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto mx-auto  text-center p-3 text-[#2e79c7] text-3xl leading-12">TypeScript 是 JavaScript 的超集(Superset)，<br>同時也支持與 ECMAScript 的協作</div>

<div class="rounded-full  mx-auto bg-[#2E79C7]   h-80  mt-10  pb-6  w-80 relative " v-click="1">
  <div class="mx-auto text-xl p-1 top-5 right-0  left-0 w-[70px] z-5 inline-block absolute">
   <img src="tslogo.png" >
  </div>  
<div class="rounded-full  mx-auto bg-[#f0f0f0]   h-48  mt-16  pb-6  right-0 bottom-4 left-0 w-48  absolute" v-click="2">
  <div class="font-bold mx-auto h-10  text-center top-14 right-0  left-0 text-[20px]  text-[#696969] absolute" >ECMAScript (ES6)</div> 
</div>

<div class="mx-auto text-xl p-1 right-0 bottom-5  left-0 w-[70px] inline-block absolute" >
  <img src="JavaScript-logo.png" >
</div>

</div>

---

  <div class="font-bold  text-center mb-10 tracking-wide  text-[#2e79c7] text-[30px] relative">  ECMAScript 始於 JavaScript 
  </div>
  
  <div class=" mx-auto h-80 w-full relative">
 
  <div class="bg-white mx-auto text-xl p-1 right-0 bottom-5 left-0 w-[200px] z-10 absolute ">
   <img src="JavaScript-logo.png" >
  </div>

  <div v-click="1">
  <Arrow x1="500" y1="200" x2="700" y2="100" color="#2c2c2c" width="2.5"/>
  <div class=" bg-white rounded-full border-4 h-[150px] shadow text-xl  p-1  top-3 right-18 w-[150px] absolute">
   <img src="Netscape_logo.svg.png" class="mx-auto mt-13 w-120px">
  </div>
  <div class="font-bold mx-auto bg-[#2e79c7] text-white text-shadow text-center text-xl  py-1 top-34 right-20 w-34 absolute">Javascript</div>
  </div>
  
  <div v-click="2">
  <Arrow x1="380" y1="200" x2="130" y2="100" color="#2c2c2c" width="2.5"/>
  <div class=" bg-white rounded-full border-4 h-[150px] shadow text-xl p-1 top-3  left-18  w-[150px]  absolute" >
   <img src="ie.png" class="mx-auto mt-4 w-80px">
  </div>
  <div class="font-bold mx-auto bg-[#2e79c7] text-white text-shadow text-center text-xl  py-1  top-34 left-22 w-30 absolute">JScript</div>
  </div>
  <div class=" h-full bg-[#f1f1f180]  w-full" v-click="3">
    <span class="font-bold right-4 bottom-4 text-[#000000CC] block absolute"> ECMAScript 標準化寫法 </span>
  </div>
  </div>
  <div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 z-3 absolute"></div>

---

  <div class="font-bold  text-left mb-10 tracking-wide  text-[#2e79c7] text-[30px] relative"> ECMAScript
  </div>
  <div class="font-bold bg-[#2e79c7] text-white text-center p-0.5 w-26">出現目的:</div>
  <div class="mt-5 px-4 text-[#3C3C3C]">
    為了解決 JavaScript 的互通性問題，一個叫做 ECMA 的組織（歐洲計算機製造商協會）開始『 標準化 』這個語言，所以誕生了 『 ECMAScript 』。
  </div>
  <div class="font-bold bg-[#2e79c7] mt-10 text-white text-center p-0.5  w-26">版本:</div>
  <div class="mt-5 px-4 text-[#3C3C3C]">
    有很多不同版本的 ECMAScript，其中最有影響力的是ES6 (也被稱為 ECMAScript 2015)。這個版本加入了很多新特性，如Arrow Function、ES Module、類等
  </div>
  
  <div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<h3 class="font-bold my-auto  mx-auto  mt-40  text-xl text-center p-3 text-[#2e79c7]">即使 JavaScript 有了 ECMAScript 規範，還是 <span class="text-[40px]">『 弱型別 』</span></h3>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<span class="font-bold bg-[#f0dc4e] text-black mb-5 p-1 w-25 block">JavaScript</span>

<span class="text-base ">範例一 : </span>

```js {2|4|6|all}
// index.js
let message = "Hello JavaScript"; // step1: type -> string

message = 666; // step2: type -> number

message = false; // step3: type -> boolean
```

<div class="mt-5 relative" >

<span class="text-base ">範例二 : </span>

```js {7|2|4-6|8|all}
// index.js
let appleCount = "1";

const addApple = (count) => {
  return count++;
};

console.log(addApple(appleCount)); // 12
```

</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div  class="font-bold  text-center mb-10 text-3xl text-[#2e79c7]" >
  <div>TypeScript 與 JavaScript 、 ECMAScript ?</div> 
</div>

<div class="rounded-full  mx-auto bg-[#F0F0F0]  h-46  mt-40  pb-6  w-46 relative ">
  <div class="rounded-full  mx-auto bg-[#2e79c7]  h-80  mt-16  pb-6  right-16 bottom-29 w-80 -z-1 relative" >
   <div class="font-bold my-auto mx-auto h-10 text-left  text-white top-5  right-0  left-0 text-[22px] w-30 block absolute" >TypeScript</div>

  <div class="my-auto space-x-2 h-15  text-white top-16 right-0 text-[14px] w-70 absolute ">
    <div class="inline-block">Type Syetem、</div>
    <div class="inline-block">Enums、</div>
    <div class="inline-block">Generics、</div>
    <div class="inline-block">Interfaces、</div>
    <div class="inline-block"> Strictness levels</div>
  </div>
  
  </div>

  <div class="font-bold my-auto mx-auto h-10 text-center  top-10 right-0  left-0  text-[26px] text-[#696969] w-30 block absolute" >ES6</div>

  <div class="mx-auto text-xl p-1 right-0 bottom-3  left-0 w-[80px] inline-block absolute">
   <img src="JavaScript-logo.png" >
  </div>  
</div>
<div>
<!-- <Arrow x1='650' y1="300" x2='860' y2='300' /> -->
<!-- <div class="mx-auto text-xl p-1 right-20 bottom-54   w-[80px] inline-block absolute">
  <img src="JavaScript-logo.png" >
</div> -->
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
 
---

<span class="font-bold bg-[#2e79c7] text-white mb-5 p-1 w-25 block">TypeScript</span>

<span class="text-base ">範例一 : </span>

```ts
// index.ts
let message: string = "Hello JavaScript"; // step1: type  string
message = 666; //
```

<img src="day2_ex1.png" class="right-10 bottom-80 w-400px absolute" >

<div class="mt-5 relative" >

<span class="text-base ">範例二 : </span>

```ts
// index.ts
let appleCount = "1";

const addApple = (count: number) => {
  return count++;
};

console.log(addApple(appleCount));
```

<img src="day2_ex2.png" class="right-10 bottom-0 w-400px absolute" >
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl">總結以上 </div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-60 inline-block"> 下集預告:<br/>TypeScript 環境設定</span></div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
