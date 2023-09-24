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
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-70 block">物件型別 Object Type</span> 
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
<div class="  rounded-sm   font-bold text-center py-1.5 px-4 top-58  left-30  w-48 absolute" :class="[($slidev.nav.clicks === 1)? 'bg-[#2F6FB0] text-white':'border-[#2F6FB0] border-dashed border-2 text-[#2F6FB0]']">
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

<div class="font-bold my-auto  mx-auto text-center p-3 text-[#2e79c7] text-3xl">基礎物件型別</div>
<div class="h-full ">
  <div class="flex h-46 mt-20 w-full items-center  justify-center relative">
    <div class="rounded-full mx-auto  h-60  text-center top-2 right-70 left-0 w-60  absolute" :class=" $slidev.nav.clicks === 1 ? 'bg-[#2F6FB0] z-3':'-z-3 bg-[#CEDCEC66]'"></div>
    <div class="rounded-full mx-auto bg-[#CAD8E64D] h-48 text-center right-0 -bottom-3 left-0 w-48  -z-1 absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}"></div>
    <div class="rounded-full mx-auto bg-[#C4E1FF33] h-68 text-center top-3 right-0 left-90 w-68 -z-2 absolute " ></div>
    <div class="font-bold mx-auto  mt-20 text-center top-2 left-50    text-23px w-45  absolute" :class=" $slidev.nav.clicks === 1 ? 'z-3 text-white':'text-[#2F6FB0]'">
      物件 <br>Object literal
    </div>
    <div class="font-bold m-auto text-center top-20  right-0 bottom-0 left-0 text-24px text-[#2F6FB0]   w-40 absolute " :class="{' opacity-25': $slidev.nav.clicks === 1}">
      陣列 array 
    </div>
    <div class="font-bold text-center right-14 right-34 bottom-0 bottom-5   text-30px  text-[#2F6FB0]  w-60   absolute" :class="{' opacity-25': $slidev.nav.clicks === 1}">
      函式 function
    </div>
  </div>
</div>

<div v-click="1"></div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left p-3 text-[#2e79c7] text-3xl">總結以上</div>

<div class="border flex flex-col h-auto mx-auto border-b-[#f1f1f1] mt-10 w-full text-[#3C3C3C]">

<div class="flex border-b-[#f1f1f1]   text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  1.  物件中的 屬性 會依照 『屬性值』或『 function 回傳值』推論出其對應型別
<span class="bg-[#2e79c7] text-xl text-white p-1 top-3 -right-4 -rotate-10 block absolute" v-click="1">型別推論</span>
</div>
<div class=" space-y-1  border-b-[#f1f1f1]  text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  <span class="w-full  block">2. 可覆寫 擁有相同 『物件屬性』 且 『相同型別』的值 </span>

<span class="bg-[#2e79c7] text-xl text-white p-1 top-5 -right-4 -rotate-10 block absolute" v-click="2">型別推論</span>

</div>

<div class=" space-y-1  border-b-[#f1f1f1]  text-left w-full py-5 px-3 text-16px relative odd:bg-gray-100">
  <span class="text- w-full  block ">3-1. 變數 可以被『任何物件』覆寫</span>
  <span class="w-full  block">3-2. 不可覆寫 擁有相同 『物件屬性』 且 『相同型別』的值 </span>
<span class="border-[#2e79c7] text-[#2e79c7] border-2 bg-white text-xl  p-1 top-5 -right-4 -rotate-10 block absolute" v-click="3">型別註解</span>

</div>

<div class=" border-b-[#f1f1f1] text-left  w-full py-5 px-3  text-16px relative odd:bg-gray-100">
  <span class="w-full  block">4-1. 新增不存在的物件屬性或方法</span>
<span class="bg-[#CE0000B3] text-xl text-white p-1 top-3 -right-4 -rotate-10 block absolute" v-click="4">兩者皆不行</span>
</div>

</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left  text-[#2e79c7] text-2xl">注意: strictNullCheck 設定 X 物件型別推論 </div>

  <div class="my-6 text-[17px] text-[#696969]">當 <span class="font-medium bg-[#ADADAD33] mx-1.5 px-1 inline-block">strictNullChecks: false;</span>物件中被賦予 nullable 的值 將會被指定爲 any，請小心使用
  </div>

```javascript

//strictNullChecks: false

let obj = {
  title : 'i am title'
  content : null, // type -> any
}

//strictNullChecks: true

let obj = {
  title : 'i am title'
  content : null, // type -> null
}

```

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left  text-[#2e79c7] text-2xl">注意: 物件 X 型別註記 ？ </div>

  <div class="my-6 text-[17px] text-[#696969]">TypeScript 認為 Object 型別指的可能是任何 Javascript 物件（Array、Function），所以只要是object型別都可以被套入
  </div>

```javascript

let userInfo: object = {
  name : 'winnie'
}

userInfo = [1, 2, 3] // 因為 Array 本身也是物件 所以不會報錯
userInfo = new Boolean(false) // 不會報錯

```

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告: <br/>函式型別 Function Types </span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

參考資料 :https://ithelp.ithome.com.tw/articles/10218941
