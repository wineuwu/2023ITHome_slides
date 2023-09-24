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
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-70 block"> 函式型別 Function Type</span> 
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
      函式 function
    </div>
    <div class="font-bold text-center opacity-25 right-14 right-34 bottom-0   bottom-5  text-30px  text-[#2F6FB0]   w-60 absolute">
     陣列 array
    </div>
  </div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[25px] w-40 inline-block"> 總結以上 </span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left p-3 text-[#2e79c7] text-[26px]">關於 Function 函式</div>

<ul class="space-y-5 mt-10 text-xl text-[#696969]">
  <li>
  1. 需針對『參數』加入『型別註解』 ， TS 在多數情況下會依照其推論出『回傳值的型別』
  </li>
  <li>
  2. 但有例外，有可能回傳值會是any，所以必需主動對該值做 型別註解。
  </li>
  <li>
  3. 只要格式正確， 可以完全『覆寫』函式物件的屬性
  </li>
  <li>
  4. 可以使用 void 來指定Function不回傳值註解
  </li>
</ul>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告:<br/>
 陣列 Array Type</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<!-- https://ithelp.ithome.com.tw/articles/10214939 -->

<!-- https://ithelp.ithome.com.tw/articles/10219539 -->
