---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day8
---

<div class="flex h-full space-x-8  mb-10 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-70 block"> 陣列 Array Type</span> 
  </div>
  <div class="h-42 w-42">
    <img src ="/tslogo.png" class="mx-auto"/>
  </div>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-center p-3 text-[#2e79c7] text-3xl">基礎物件型別</div>
<div class="h-full ">
  <div class="flex h-46 mt-20 w-full items-center  justify-center relative">
    <div class="rounded-full mx-auto bg-[#C4E1FF33] h-60  text-center top-2 right-70 left-0 w-60  absolute " ></div>
    <div class="rounded-full mx-auto  bg-[#2F6FB0] h-48 text-center right-0 -bottom-3 left-0   w-48  z-3 absolute" ></div>
    <div class="rounded-full mx-auto bg-[#C4E1FF33] h-68 text-center top-3 right-0 left-90 w-68 -z-2 absolute " ></div>
    <div class="font-bold mx-auto  mt-20 text-center opacity-25 top-2    left-50 text-23px  text-[#2F6FB0] w-45 absolute">
      物件 <br>Object literal
    </div>
    <div class="font-bold m-auto text-center text-white  top-20 right-0 bottom-0 left-0 text-24px   text-[#2F6FB0] w-40 z-3 absolute">
      陣列 array
    </div>
    <div class="font-bold text-center opacity-25 right-14 right-34 bottom-0   bottom-5  text-30px  text-[#2F6FB0]   w-60 absolute">
     函式 function 
    </div>
  </div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[25px] w-40 inline-block"> 總結以上 </span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left p-3 text-[#2e79c7] text-[26px]">陣列 Array X 型別推論</div>

<div class="border flex flex-col h-auto mx-auto border-b-[#f1f1f1] mt-10 w-full text-[#3C3C3C]">

<div class="flex border-b-[#f1f1f1]   text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  1. 當陣列中的值 皆為同型別時， 會以 <span class="inline-block bg-white px-2 py-0.5 mx-2">Type[]</span> 的方式表示。

</div>
<div class=" space-y-1  border-b-[#f1f1f1]  text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  <span class="w-full  block mb-2">2.當 陣列中的值 『有多個型別』或『有多個屬性且不同型別的物件』時，TS 對於這一類型的陣列，會以 <span class="inline-block bg-[#f1f1f1] p-1">union</span>方法來進行型別推論</span>

```typescript
let arr = ["a", false, 1]; // (string| boolean | number)[]
```

</div>
<div class=" space-y-1  border-b-[#f1f1f1]  text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  <span class="w-full  block">3. ts 中的 <span class="inline-block bg-white px-2 py-0.5 mx-2">?</span>表示某個屬性或參數為選用的 </span>
</div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left p-3 text-[#2e79c7] text-[26px]">陣列 Array X  型別註解</div>

<div class="border flex flex-col h-auto mx-auto border-b-[#f1f1f1] mt-10 w-full text-[#3C3C3C]">

<div class=" space-y-1  border-b-[#f1f1f1]  text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  <span class="text- w-full  block ">1. 『空陣列值』必須 對該變數做『型別註解』，來避免 『any』值的出現。
</span>

</div>

<div class=" border-b-[#f1f1f1] text-left  w-full py-5 px-3  text-16px relative odd:bg-gray-100">
  <span class="w-full  block">2. 當陣列裡的值沒有你要求的型別，可以用 <span class="inline-block bg-[#f1f1f1] p-1">union</span> 來作積極的型別註解</span>
</div>

</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告:<br/>
Tuples 元組</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<!-- https://ithelp.ithome.com.tw/articles/10214939 -->

<!-- https://ithelp.ithome.com.tw/articles/10219539 -->
