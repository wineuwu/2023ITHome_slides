---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day15
---

<div class="flex h-full space-x-8  mb-10 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 block">特殊型別 any & unknown type</span> 
  </div>
  <div class="h-42 w-42">
    <img src ="/tslogo.png" class="mx-auto"/>
  </div>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" font-bold mx-auto mt-30 text-[#2e79c7]  text-center  p-4  text-3xl w-50 "><tabler-alert-triangle class="mr-5 inline-block "/>注意 </div>

<div class="text-center text-[#696969] mt-5">
『 any 型別 』會造成 TypeScript 跳過型別檢測，使變數『容易引發非預期行為』的機率上升。
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  text-left    text-[#2e79c7] text-[24px] w-100" >any 出沒的時機</div>

<div class="flex mt-10 space-x-5">
  <div class="w-1/2 p-1 ">
    <span class="block p-1 text-[14px] bg-[#2e79c7] text-white w-30 text-center mb-5">延遲性指派</span>

```javascript
let a; // type -> any
```

  </div>
  <div class="w-1/2 p-1 ">
    <span class="block p-1 text-[14px] bg-[#2e79c7] text-white w-30 text-center mb-5">一般函式中的參數</span>

```javascript
let sum = (num1, num2) => {
  return num1 + num2;
};
```

  </div>
</div>
<div class="flex mt-10 space-x-5">
  <div class="w-1/2 p-1 ">
    <span class="block p-1 text-[14px] bg-[#2e79c7] text-white w-30 text-center mb-5">函式回傳之值</span>

```javascript
(method) JSON.parse(...: any) => any) | undefined): any
```

  </div>
  <div class="w-1/2 p-1 ">
    <span class="block p-1 text-[14px] bg-[#2e79c7] text-white w-30 text-center mb-5">未註解的空陣列</span>

```javascript
let arr = []; // type => any[]
```

  </div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" flex space-x-10  mt-40 justify-center">

<div class="font-medium bg-[#2e79c7] border-[#2e79c7] border-3   text-center p-4 text-2xl w-45" :class="$slidev.nav.clicks === 0? '  bg-[#2e79c7] text-white ':'text-[#2e79c7] bg-white'">any</div>
<div class="bg-[#2e79c7]  text-white text-center  text-2xl w-1"></div>
<div class="font-medium   text-center border-[#2e79c7] p-4 border-3 text-2xl w-45" :class="$slidev.nav.clicks === 1? 'bg-[#2e79c7] text-white':'text-[#2e79c7]'">unknown</div>

</div>

<div class="w-116 text-center text-white absolute top-20 bottom-0 left-0 right-0 m-auto text-lg font-medium h-10 leading-10 bg-[#2e79c7]" v-click='1'>
unknown 相對 any 來說，是一種更安全的型別機制
</div>

<div class="w-116 text-center bg-white border-2 absolute top-20 bottom-0 left-0 right-0 m-auto text-lg font-medium h-10 leading-10 text-[#2e79c7] border-[#2e79c7]" v-if="$slidev.nav.clicks === 0">如難以避免型別出現 any， 那開發者也應主動型別註解</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  mx-auto mt-35 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-50 inline-block"> 總結以上
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" space-y-4 text-[#2e79c7]">
  <div class="font-bold text-left mb-10  tracking-wide text-[#2e79c7] text-[26px] relative"> 總結以上
  </div>
  <div class="space-y-7 mt-20 text-[#696969]">
  <div >
   1.  只要當變數被註解為 any 或 unknown，該變數照樣都可以接收 <span class="text-[#2e79c7] font-bold">『 任意型別的值 』</span>
  </div>
  <div>
   2.  但 unknown 型別的變數，在大多情境下<span class="text-[#2e79c7] font-bold"> 不得將其值指派到 任意型別 </span>( 除了any 或 unknown 型別 )
  </div>
  <div>
   3.  除非透過 <span class="text-[#2e79c7] font-bold">『 控制程式判斷流程限縮 unknown 型別至某型別 』 </span>或者 明確使用<span class="text-[#2e79c7] font-bold">『型別斷言方式』 </span>，就可以進行指派
  </div>

  </div>
  
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" space-y-4 text-[#2e79c7]">
  <div class="font-bold text-left mb-10  tracking-wide text-[#2e79c7] text-[26px] relative"> unknown 型別的複合型別型態
  </div>
  <div class="space-y-7 mt-20 text-[#696969]">
  <div class=" my-5">
   4.  任何與 unknown 型別進行 intersection 過後的型別，則會吸收掉 unknown
  </div>

```javascript
type UnionType = unknown & string // type => string

```

  <div class="pb-5">
   5.  任何與 unknown 型別進行 union 型別 且同時不為 any 型別時，則 unknown 會吸收掉其型別
  </div>
  
```javascript
type U = unknown | string;
// => unknown

type V = unknown | any;
// => any

```

</div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-30 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-50 inline-block"> 下集預告:  Interface
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

