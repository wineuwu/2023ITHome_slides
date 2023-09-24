---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day6
---

<div class="flex h-full space-x-8  mb-10 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-70 block">TS型別類型 - 原始資料型別</span> 
  </div>
  <div class="h-42 w-42">
    <img src ="/tslogo.png" class="mx-auto"/>
  </div>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="rounded-full m-auto bg-[#CEDCEC66] h-64  text-center  top-0 right-0  bottom-0 left-0 w-64 -z-3 absolute " ></div>
<div class="font-bold mx-auto  mt-50  text-center text-24px  text-[#2F6FB0] " >
  TypeScript <br>型別類型
  
</div>

<div class="  rounded-md font-bold  text-center py-1.5  px-6   top-28 left-40 w-50 absolute" :class="[($slidev.nav.clicks === 1)? 'bg-[#2F6FB0] text-white':'border-[#2F6FB0] border-dashed border-2 text-[#2F6FB0]']">
  原始資料型別 (Primitive Type)  
  <img src="JavaScript-logo.png" class="-top-5 -left-5 w-10 absolute ">
</div>
<div class=" border-dashed rounded-md font-bold border-[#2F6FB0] border-2 text-center py-1.5  px-4 top-58  left-30 text-[#2F6FB0] w-48 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  物件型別 <br>(Object Type)
  <img src="JavaScript-logo.png" class="-top-5 -left-5 w-10 absolute ">
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0] border-2 shadow-inner  text-center  py-1.5 px-4 top-90 left-34  text-[16px] text-[#2F6FB0] w-55 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  TypeScript 擴充型別 (Enum、Tuple)
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center  py-2 px-4 top-20 right-32 text-[16px] text-[#2F6FB0] w-60 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  明文型別<br> (Literal Type)
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center  py-1.5 px-4 top-46 right-18 text-[16px] text-[#2F6FB0] w-62 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  特殊型別 <br>(any、unknown、never) 
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center py-1.5 px-4 right-18 bottom-50 text-[16px] text-[#2F6FB0] w-64 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  複合型別 <br>(union、intersection)
</div>

<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center py-1.5 px-4 right-26 bottom-22 text-[16px] text-[#2F6FB0] w-64 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  通用型別 <br>(Generics)
</div>

<div v-click="1"></div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

  <div class="font-bold text-left mb-5  tracking-wide text-[#2e79c7] text-[26px] relative"> 
  原始資料型別 (Primitive Type) 
  </div>

  <ul class="space-y-4 mt-5 text-[#696969] text-[22px]">
  <li > 字串 String </li>
  <li > 數字 Number  </li>
  <li > 布林值 Boolean </li>
  <li > Null</li>
  <li > Undefined</li>
  </ul>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

  <div class="font-bold text-left mb-5  tracking-wide text-[#2e79c7] text-[26px] relative"> 
   總結以上，需注意 
  </div>

<div class="my-8 text-[16px] text-[#696969]">1.使用 建構函式 的 Boolean 建立的物件不是布林值</div>

```javascript
let boolObj = new Boolean(false); // type Boolean
let byBoolean = Boolean(false); // type boolean
```

---

  <div class="font-bold text-left mb-5  tracking-wide text-[#2e79c7] text-[26px] relative"> 
  關於 Nullable Type需注意 
  </div>

  <div class="my-6 text-[16px] text-[#696969]">1.宣告 nullable types 時，為避免 any 值出現，需指定 明確使用 『型別註解』 來指定型別</div>

```javascript
let nothing: undefined = undefined ;

let nothing2: null = null;

```

  <div class="my-6 text-[16px] text-[#696969]">2.當開啟 <span class="font-medium bg-[#ADADAD33] mx-1.5 px-1 inline-block">strictNullChecks: true;</span>將視為不同的類型，不能直接賦值給其他變數</div>

```javascript


   //strictNullChecks: false

  let userName: string = undefined ;
  let userAge: number  = null;


 //strictNullChecks: true;

  let userName: string | undefined = undefined ;
  let userAge: number | null = null;

```

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---


<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告: <br/>物件型別 Object Type</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
