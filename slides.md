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
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-54 block">interface 介面的擴展 </span> 
  </div>
  <div class="h-42 w-42">
    <img src ="/tslogo.png" class="mx-auto"/>
  </div>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" flex space-x-10  mt-30 justify-center">

<div class="font-medium bg-[#2e79c7] border-[#2e79c7] border-3   text-center p-4 text-[18px] w-118 text-[#2e79c7] bg-white relative" ><span class="text-2xl">介面的擴展</span> <br>(Interface Extension / Inheritance)</div>

</div>

<div class="w-118 text-center text-white absolute top-20 bottom-0 left-0 right-0 m-auto text-[16px] font-medium h-17  py-3 bg-[#2e79c7]" v-click="1">
可以透過 extends 關鍵字
來將宣告好的 interface 介面<br>『擴充』給 『另一個介面』 進行延伸
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-28 text-center p-3.5 px-8 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7]  text-white text-center p-1 text-[20px] w-125 inline-block"> 如果不同的介面，兩者『同時有重複』的屬性名稱 ？
</span> </div>

<div class="text-center text-[#696969] mt-8" v-click="1">
<div class="text-center text-[#696969] " >
  不同的介面，<span class="inline-block   text-[#2e79c7]  w-36 text-center font-medium">『可以互有重複』</span>的屬性名稱 
  ，但各自對應相同屬性的 <span class="inline-block   text-[#2e79c7]  w-50 text-center font-medium">『 型別不能互相衝突 』</span>。
</div>

<div class="text-center  text-[#696969] mt-3" v-click="1">
只要其中有<span class="inline-block   text-[#2e79c7]  w-40 text-center font-medium">『 介面互不相容 』</span>，就不能進行擴展的動作。
</div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  text-left  mt-4 text-[#2e79c7] text-[22px] w-100" > 介面 Interface V.S. 型別 Type
</div>

<div class=" text-[#696969] mt-5 mb-10 leading-8">
從介面擴展（Interface Extension）的介紹，
就可以區分一點『interface 介面』跟『型別系統』的主要差別 :
</div>

  <div class="flex items-center shadow w-200 border-[#F1f1f1] border-0.5 h-15 my-8" v-click='1'>
    <span class="block p-2  p-4.5 text-[16px] bg-[#2e79c7] text-white w-34 text-center ">interface</span>
    <div class=" text-[#696969] my-5 text-[16px] pl-3">
     與『樂高積木』的概念很像，可以擴充設計、組裝出更複雜的功能
    </div>
  </div>
  <div class="flex items-center shadow w-200 border-[#F1f1f1] border-0.5 my-8 h-15" v-click='2'>
    <span class="block p-4.5 text-[16px] bg-[#2e79c7] text-white w-50 text-center ">型別化名 type</span>
    <div class=" text-[#696969] my-5 text-[16px] pl-3">
      主要為 『靜態的資料』型態，型別一但被定義出來則恆為固定的狀態。儘管可以利用型態的複合（intersection 與 union），也是創造出新的靜態型別
    </div>
  </div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  mx-auto mt-35 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-50 inline-block"> 總結以上
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-30 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-100 inline-block"> 下集預告:  Interface 的 函式超載
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
