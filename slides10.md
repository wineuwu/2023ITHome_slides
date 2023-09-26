---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day10
---

<style>
</style>

<div class="flex h-full space-x-8  mb-10 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-70 block">Tuple 元組</span> 
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

<div class="  border-dashed rounded-md font-bold  border-[#2F6FB0] border-2 text-center  py-1.5 px-6 top-28 left-40 text-[#2F6FB0] w-50 absolute "  :class="{' opacity-25': $slidev.nav.clicks === 1}">
  原始資料型別 (Primitive Type)  
  <img src="JavaScript-logo.png" class="-top-5 -left-5 w-10 absolute ">
</div>
<div class="  border-dashed   rounded-sm font-bold border-[#2F6FB0] border-2 text-center  py-1.5  px-4 top-58 left-30 text-[#2F6FB0] w-48 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}" >
  物件型別 <br>(Object Type)
  <img src="JavaScript-logo.png" class="-top-5 -left-5 w-10 absolute ">
</div>
<div class="  rounded-md font-bold shadow-inner  text-center  py-1.5 px-4 top-90 left-34  text-[16px]  w-55 absolute" :class="[($slidev.nav.clicks === 1)? 'bg-[#2F6FB0] text-white':'border-[#2F6FB0] border-dashed border-2 text-[#2F6FB0]']">
  TypeScript 擴充型別 (Tuple、Enum)
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

<div class="font-bold my-auto  mx-auto text-left  text-[#2e79c7] text-3xl">元組 Tuple</div>
<span>
<div class="mt-5 text-[#696969]">
Tuples 元組 可以想成是一個『 嚴格檢查格式型別』的陣列，陣列長度為『固定』且 可以為『 混合型態 』的陣列。
</div>
</span>
<div class=" flex mt-10 text-[40px] justify-center ">
    <div class="flex space-x-16 bg-[#ECF5FF] mx-5 p-4 w-140 justify-center inline-block relative">
    <div class=" font-medium h-14 text-shadow text-center py-4.5 text-2xl w-16   " :class="(idx === 3)? 'text-[#2e79c7] ': 'bg-[#2e79c7] text-white'" :key="i" v-for="i,idx in ['T1', 'T2', 'T3','...', 'Tn']" >
   {{i}}
    </div>
    <div class=" font-medium  bg-[#696969]  h-14 text-center text-white text-shadow text-xl py-3 -left-12  w-18 absolute" v-click="1">string</div>
    <div class=" font-medium  bg-[#696969]  h-14 text-center text-white text-shadow text-xl py-3   left-14 w-22 absolute" v-click="3">number</div>
    </div>
</div>

<div class=" flex text-[40px] justify-center">
    <div class="flex space-x-16 mx-5 p-4 w-140 justify-center  inline-block">
    <div class=" bg-white  font-medium h-10 text-center py-3 text-2xl text-[#696969]   w-16   relative" v-for="i in 5" :key="i">
      <div class="border-dashed border-l-4 border-[#696969] h-10 inline-block">
      </div>
      <div class="border-b-[transparent] border-r-[transparent] border-l-[transparent] border-t-[#696969]  border-t-12 border-b-12 border-l-10 border-r-10 h-0 -bottom-8 left-[17px] w-0 absolute"></div>
    </div>
    </div>
</div>

<div class=" flex mt-6 text-[40px] justify-center">
    <div class="flex space-x-16 bg-[#F0F0F0B3] mx-5 p-4 w-140 justify-center inline-block relative ">
    <div class=" font-medium  h-14 text-center py-3 text-2xl text-[#696969] w-16   " v-for="i,idx in ['V1', 'V2', 'V3','...', 'Vn']"
    :class="(idx === 3)? '': 'bg-white'" :key="i">
   {{ i}}
    </div>
    <div class=" font-medium  bg-[#01B468]  h-14 text-center text-white text-shadow py-3 -left-12 text-2xl  w-18 absolute" v-click="2">'a'</div>
    <div class=" font-medium  bg-[#FF2D2D]  h-14 text-center text-white text-shadow py-3 left-16 text-2xl  w-18 absolute" v-click="4">'1'</div>
  </div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left  text-[#2e79c7] text-[26px]"> Tuple 元組 X  型別註解</div>

<div class="my-5 text-[#696969]">
 使用 『 Tuple元組 』時，須主動使用 『型別註解』， 而 『被指派元組型別』 的變數也需主動註解。
</div>

```js

let userInfo :[string, string, boolean] = ['winnie', '26', false]

userInfo  = ['26', 'winnie', true] // pass

userInfo  = [false ,'winnie', '26'] // ts error


```

<div class="my-4 text-[#696969]">
 但變數註解多了，有可能會碰到下列情境 :
</div>

```js

let userInfo :[string, string, boolean] = ['winnie', '26', false]

let userInfo2 :[string, string, boolean] = ['jack', '15', true]

let userInfo2 :[string, string, boolean] = ['eric', '10', true]

```

---

<div class="font-bold my-auto  mx-auto text-left  text-[#2e79c7] text-[26px]"> 型別化名(Type Alias)</div>

<div class="my-4 tracking-wide text-[#696969E6]">
 以 <span class="bg-[#f1f1f1] p-1 inline-block">type</span> 關鍵字 為『 現有的型別』或 『複合型別』定義一個新名稱，使能夠更容易理解 『複雜的型別』結構 
</div>

```js

type [string, string, boolean] = userInfoType

let userInfo :userInfoType = ['winnie', '26', false]

let userInfo2 :userInfoType = ['jack', '15', true]

let userInfo2 :userInfoType = ['eric', '10', true]

```

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 陣列與元組的差異</span> </div>

---

<div class="font-bold my-auto  mx-auto text-left p-3 text-[#2e79c7] text-3xl">總結以上</div>

<div class="border flex flex-col h-auto mx-auto border-b-[#f1f1f1] mt-10 w-full text-[#3C3C3C]">

<div class=" space-y-1  border-b-[#f1f1f1]  text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  <span class="text- w-full  block ">1. 只能使用 『型別註解』來宣告型別
</span>
 <span class="bg-white border-[#2e79c7] border-2 text-xl p-1  top-5 -right-4 text-[#2e79c7] -rotate-10 block absolute  " v-click="3"> Tuple元組</span>
</div>

<div class=" border-b-[#f1f1f1] text-left  w-full py-5 px-3 text-16px relative odd:bg-gray-100 ">
  <span class="w-full  block"> 2.『 陣列長度』沒有一定限定外，順序也不限定 </span>
  <span class="bg-[#2e79c7] text-xl text-white p-1 px-2 top-5 -right-4 -rotate-10 block absolute" v-click="2">陣列型別</span>
</div>

<div class=" border-b-[#f1f1f1] text-left  w-full py-5 px-3  text-16px relative  odd:bg-gray-100  ">
  <span class="w-full  block">3.『 陣列值的順序及型別 』必須完全吻合 </span>
<span class="bg-white border-[#2e79c7] border-2 text-xl p-1  top-5 -right-4 text-[#2e79c7] -rotate-10 block absolute  " v-click="3"> Tuple元組</span>

</div>

</div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告: <br/>列舉 Enum Type
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl" ><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 請問 Tuple 你都怎麼念？
</span> </div>

  <img src ="/tuple2.png" class=" top-40 left-55   w-[520px] block absolute" v-click="1"/>

  <img src ="/ikea.png" class=" top-40 left-55   w-[520px] block absolute" v-click="2"/>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---
