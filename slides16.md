---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day16
---

<div class="flex h-full space-x-8  mb-10 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-54 block">interface X 介面宣告 </span> 
  </div>
  <div class="h-42 w-42">
    <img src ="/tslogo.png" class="mx-auto"/>
  </div>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-center mt-5 text-[#2e79c7] text-2xl">Interface 後續介紹內容</div>

<div class="h-full ">
  <div class="flex h-46 mt-14 w-full items-center  justify-center relative">
    <div class="rounded-full mx-auto bg-[#CEDCEC66] h-55  text-center top-5 right-90 left-0 w-55 -z-3 absolute" ></div>
    <div class="rounded-full mx-auto bg-[#CAD8E64D] h-55 text-center right-0 top-2 left-0 w-55  -z-1 absolute" ></div>
    <div class="rounded-full mx-auto bg-[#C4E1FF33] h-57 text-center top-5 right-0 left-100 w-57 -z-2 absolute " ></div>
    <div class="font-bold mx-auto  text-center  left-33 text-23px text-[#2F6FB0] top-22   w-58 absolute " >
     interface <br>
     介面宣告 
    </div>
    <div class="font-bold m-auto left- text-center  top-25 right-0 bottom-0 left-0 text-20px text-[#2F6FB0]  w-55 absolute ">
     介面 vs 型別系統 
    </div>
    <div class="font-bold text-center  right-28 bottom-0   top-24  text-20px  text-[#2F6FB0]  w-60   absolute">複合型別 <br>
    (union / intersection)
    </div>

  </div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-30 text-center  text-[#2e79c7] text-3xl"><span class="text-center   p-1 text-[#2e79c7] text-[26px] w-80 inline-block"> 型別化名(Type Alias)</span> </div>
<div class="my-5 text-center text-[#696969] text-18px">
  使用主要目的就是把複雜格式（尤其是明文格式）的型別進行<span class="text-[#2e79c7] font-bold">程式碼簡化</span>與 <span class="text-[#2e79c7] font-bold">抽象化</span>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  text-left  mt-4 text-[#2e79c7] text-[22px] w-100" > Interface 介面 定義與種類</div>

<div class=" text-[#696969] mt-5 mb-10">
宣告方式可以藉由關鍵字 interface 來進行宣告，裡面的定義需為：
</div>

  <div class="flex items-center shadow w-130 border-[#F1f1f1] border-0.5 h-8 my-8" v-click='1'>
    <span class="block p-1 text-[16px] bg-[#2e79c7] text-white w-30 text-center ">物件格式</span>
    <div class=" text-[#696969] my-5 text-[16px] pl-3">
      即 JSON 格式，主要在裡面定義『 屬性與型別 』
    </div>
  </div>
  <div class="flex items-center shadow w-160 border-[#F1f1f1] border-0.5 my-8 h-8" v-click='2'>
    <span class="block p-1 text-[16px] bg-[#2e79c7] text-white w-30 text-center ">單一函式格式</span>
    <div class=" text-[#696969] my-5 text-[16px] pl-3">
      不用寫任何屬性，單純以函式表示，同時也不一定要定義函式名稱
    </div>
  </div>
  <div class="flex h-8 items-center shadow w-130 border-[#F1f1f1] border-0.5 my-8" v-click='3' v-if="$slidev.nav.clicks !== 4">
    <span class="block p-1 text-[16px] bg-[#2e79c7] text-white w-30 text-center ">複合格式</span>
    <div class=" text-[#696969] my-5 text-[16px] pl-3">
      也就是將『物件格式』與『單一函式格式』複合一起
    </div>
  </div>
  <div v-click="4"></div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  mx-auto mt-35 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-50 inline-block"> 總結以上
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" space-y-4 text-[#2e79c7] leading-10">
  <div class="font-bold text-left mb-10  tracking-wide text-[#2e79c7] text-[26px] relative"> 總結以上
  </div>
  <div class="space-y-7 mt-20 text-[#696969] text-xl tracking-wide">
  <div >
   1. 變數值的內容必須<span class="text-[#2e79c7] font-bold"> 完全符合定義好的型別格式</span>
  </div>
  <div class="leading-8">
   2. 當變數為『物件』且作為『參數』時需注意 : <br>
   <div class="mt-4 pl-5">如果該變數<span class="text-[#2e79c7] font-bold"> 沒有主動 『型別註解』</span>，只要該變數<span class="text-[#2e79c7] mt-4 font-bold"> 至少有符合介面的格式</span>，依然可以通過參數對於變數值的驗證
   </div>

  </div>
  <div>
   3.  如果想避免此情境的發生，任何變數需要定義物件時，同時也<span class="text-[#2e79c7] font-bold mt-1">必須進行主動使用的型別註解 <span class="text-[#2e79c7] font-bold mt-1 inline-block pl-5 mt-4">或 使用interface的動作。</span></span>
   
  </div>

  </div>
  
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-30 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-100 inline-block"> 下集預告:  Interface 的 擴展
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
