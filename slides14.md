---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day13
---

<style>
</style>

<div class="flex h-full space-x-8  mb-10 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 block">特殊屬性 Never Type</span> 
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
<div class="  border-dashed   rounded-sm font-bold border-[#2F6FB0] border-2 text-center  py-1.5  px-4 top-58 left-30 text-[#2F6FB0] w-48 absolute"  :class="{' opacity-25': $slidev.nav.clicks === 1}" >
  物件型別 <br>(Object Type)
  <img src="JavaScript-logo.png" class="-top-5 -left-5 w-10 absolute ">
</div>
<div class="  bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6]  border-2  shadow-inner text-center py-1.5 px-4  top-90  left-34  text-[#2F6FB0] text-[16px]  w-55 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  TypeScript 擴充型別 (Tuple、Enum)
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center  py-2 px-4 top-20 right-32 text-[16px] text-[#2F6FB0] w-60 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  明文型別<br> (Literal Type)
</div>
<div class=" rounded-md font-bold  shadow-inner text-center  py-1.5 px-4 top-46 right-18 text-[16px] text-[#2F6FB0] w-62 absolute" :class="[($slidev.nav.clicks === 1)? 'bg-[#2F6FB0] text-white':'border-[#2F6FB0] border-dashed border-2 text-[#2F6FB0]']">
  特殊型別 <br>(any、unknown、never) 
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center py-1.5 px-4 right-18 bottom-50 text-[16px] text-[#2F6FB0] w-64 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
  複合型別 <br>(union、intersection)
</div>

<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center py-1.5 px-4 right-26 bottom-22 text-[16px] text-[#2F6FB0] w-64 absolute " :class="{' opacity-25': $slidev.nav.clicks === 1}">
  通用型別 <br>(Generics)
</div>

<div v-click="1"></div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  mx-auto mt-35 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-2  w-70 inline-block">關於 Never Type
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" font-bold mx-auto mt-20 text-center  p-4 text-[#2e79c7] text-3xl w-120 ">在函式或方法執行時</div>

<div class=" flex space-x-10  mt-10 justify-center">
<div class="font-medium   text-center border-[#2e79c7] p-4 border-3 text-2xl w-76" :class="$slidev.nav.clicks === 0? 'bg-[#2e79c7] text-white':'text-[#2e79c7]'">無法跳脫出該函式或方法</div>
<div class="bg-[#2e79c7]  text-white text-center  text-2xl w-1"></div>
<div class="font-medium bg-[#2e79c7] border-[#2e79c7] border-3   text-center p-4 text-2xl w-70" :class="$slidev.nav.clicks === 1? '  bg-[#2e79c7] text-white ':'text-[#2e79c7] bg-white'">出現例外結果中斷執行</div>

</div>

<div v-click='1'></div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<a class="text-center font-medium text-[26px] w-100 block mx-auto mt-50 text-[#2e79c7] " href="https://www.typescriptlang.org/docs/handbook/release-notes/typescript-2-0.html#the-never-type" target="_blank"> TypeScript Document : never </a>

---

<div class="font-bold my-auto  mx-auto text-left p-3 text-[#2e79c7] text-[26px]">總結以上</div>
<div class="flex mt-10 h-70">
  <div class="w-440px relative">
    <div class="w-50 h-50  bg-[#2e79c7] text-white  rounded-full inline-block absolute top-0 bottom-0 left-0 my-auto text-cneter" >
      <span class='absolute left-5 top-8 text-center font-medium'>所有型別<br>(number、string ...)</span>
    </div>
    <div class="w-25 leading-25  text-center rounded-full inline-block font-medium absolute bottom-13 left-12  bg-white text-[16px] text-[#2e79c7]" >
      Never Type
    </div>
    <div v-click='1'>
    <div class="w-30 p-3 text-[#2e79c7] text-[50px] absolute right-30 top-24">=</div>
    <div class="w-30 p-3 bg-red text-white absolute right-12 top-30">Throw Error</div>
    </div>
  </div>
 
  <ul class="space-y-5 mt-5 text-[18px] text-[#696969] w-420px" >
    <li >
     never 是 所有型別的 『 子類型別(subtype) 』， 但 never 中 『 不包含 』 所有型別
    </li>
    <li v-if="$slidev.nav.clicks > 0">
    2. 因爲是 所有型別的 『 子類型別(subtype) 』，當拋出 『 Error錯誤 』時，『 擁有型別的變數 』也可以被指派為 『 Error 錯誤 』
    </li>
    <li v-click="2">
    3. 如果函式被『 主動註解 』為 never 型別，必須確保該『 函式不會有任何結束的執行點 』
    </li>

  </ul>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-30 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告: <br/>特殊型別 any & unknown type
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
