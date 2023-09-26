---
theme: default
background:
class: text-center
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day11
---

<style>
</style>

<div class="flex h-full space-x-8  mb-10 justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3 text-[#2e79c7] text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-70 block">列舉 Enum Type</span> 
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

<div class="  border-dashed rounded-md font-bold  border-[#2F6FB0] border-2 text-center  opacity-25 py-1.5 px-6 top-28 left-40 text-[#2F6FB0] w-50 absolute" >
  原始資料型別 (Primitive Type)  
  <img src="JavaScript-logo.png" class="-top-5 -left-5 w-10 absolute ">
</div>
<div class="  border-dashed   rounded-sm font-bold border-[#2F6FB0] border-2 text-center  opacity-25  py-1.5 px-4 top-58 left-30 text-[#2F6FB0] w-48 absolute" >
  物件型別 <br>(Object Type)
  <img src="JavaScript-logo.png" class="-top-5 -left-5 w-10 absolute ">
</div>
<div class="  rounded-md font-bold bg-[#2F6FB0]  shadow-inner  text-center text-white py-1.5 px-4  top-90  left-34 text-[16px] w-55 absolute">
  TypeScript 擴充型別 (Tuple、Enum)
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center  opacity-25 py-2 px-4 top-20 right-32 text-[16px] text-[#2F6FB0] w-60 absolute" >
  明文型別<br> (Literal Type)
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center  opacity-25 py-1.5 px-4 top-46 right-18 text-[16px] text-[#2F6FB0] w-62 absolute" >
  特殊型別 <br>(any、unknown、never) 
</div>
<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center opacity-25 py-1.5 px-4 right-18 bottom-50 text-[16px] text-[#2F6FB0] w-64 absolute" >
  複合型別 <br>(union、intersection)
</div>

<div class="bg-white border-dashed rounded-md font-bold border-[#2F6FB0e6] border-2 shadow-inner text-center opacity-25 py-1.5 px-4 right-26 bottom-22 text-[16px] text-[#2F6FB0] w-64 absolute">
  通用型別 <br>(Generics)
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left  text-[#2e79c7] text-3xl">
列舉 Enum Type
</div>

<div class="mt-5 text-[#696969]">
Enum 可以稱作 『列舉』或『枚舉』，它主要將『相同類型的常數』集結為一個有描述性的名稱，使得這些常數值更加組織化和方便管理。
</div>

<div class=" mt-5 tracking-wide text-[#696969E6]">
  <!-- shape -->
  <div class="flex" v-click="1">
  <div class="flex flex-wrap space-y-4 bg-[#2F6FB0E6] h-40 p-3 w-40 scale-75 justify-around">
    <div class="bg-white h-12 mt-3 w-12"></div>
    <div class="bg-white rounded-full h-12 w-12"></div>
    <div class="border-b-[transparent] border-r-[transparent] border-l-[transparent] border-t-white  border-t-40 border-b-40 border-l-25 border-r-25 h-0  w-0 "></div>
    <div class=" bg-white h-10 w-16"></div>
  </div>
    <div class="ml-20 w-30 relative">
      <div class="my-auto bg-[#2F6FB0] h-6 top-0 bottom-0 w-15 inline-block absolute"></div>
      <div class="border-b-[transparent] border-r-[transparent] border-l-[transparent] my-auto border-t-[#2F6FB0]  border-t-40 border-b-40 border-l-25 border-r-25 h-0 top-0 right-0 bottom-0 w-0 -rotate-90 inline-block absolute"></div>
    </div>
    <div class="space-y-4 h-40 pt-12">
      <div>1.共通性 : 同為『形狀』一員</div>
      <div>2.獨特性 : 擁有『不同形狀』樣式，元素不重複 </div>
    </div>
  </div>
  <!-- color -->
   <div class="flex" v-click="2">
    <div class="border-0.5 shadow w-40 scale-75 ">
      <div class=" flex space-x-2 pt-8 pb-1.5 justify-center">
        <div class=" bg-[#F07167] h-10  w-10"></div>
        <div class=" bg-[#01B468]	h-10   w-10 "></div>
      </div>
      <div class="flex space-x-2 pt-1.5 pb-8 justify-center">
        <div class=" bg-[#FFAF60] h-10  w-10"></div>
        <div class=" bg-[#00AFB9]	h-10   w-10 "></div>
      </div>
    </div>
    <div class="ml-20 opacity-90 w-30 relative">
      <div class="my-auto bg-[#2F6FB0] h-6 top-0 bottom-0 w-15 inline-block absolute"></div>
      <div class="border-b-[transparent] border-r-[transparent] border-l-[transparent] my-auto border-t-[#2F6FB0]  border-t-40 border-b-40 border-l-25 border-r-25 h-0 top-0 right-0 bottom-0 w-0 -rotate-90 inline-block absolute"></div>
    </div>
    <div class="space-y-4 h-40 pt-12">
      <div>1.共通性 : 同為『 正方形 』一員</div>
      <div>2.獨特性 : 擁有『不同顏色 』 </div>
    </div>
  </div>

</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="my-5 text-[#696969]">
  Enum 可以藉由 TypeScript 的 <span class="bg-[#f1f1f1] p-1 inline-block">enum</span>  關鍵字進行定義，且可以使用『型別註解』 宣告給變數
  </div>

```javascript

// Enum Type -> Shape

enum Shapes {
  Square,
  Circle,
  Triangle,
  Rectangle
}

let smSquare :Shapes = Shapes.Square;

```

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="my-5 text-[#696969]">
 在定義列舉型別時，其中元素可以以<span class="bg-[#f1f1f1] p-1 inline-block">＝</span> 的方式 進行賦值，否則定義的每個 Enum 常數都會被自動分配一個數值

</div>

```javascript
enum  SquareColors {
  Red = '#F07167',
  Green = '#00AFB9' ,
  Orange, = '#FFAF60'
  Blue = '#2F6FB0'
}

let squareColor: SquareColors = SquareColors.Red;
console.log(squareColor); // '#F07167'

```

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto  mx-auto text-left  text-[#2e79c7] text-[26px]"> Enum 列舉 中的 反向性查找 </div>

<div class="my-4 tracking-wide text-[#696969E6]">
 Enum 列舉 具有『反向性查找』的特性，可以藉由 Enum列舉 中 『常數的名稱』 查找 『常數的值』，反之，也可以使用 『常數的值』 來查找 對應名稱
</div>

```js

enum StatusCode {
    Ok = 200,
    NotFound = 404,
    InternalServerError = 500
}

// 用名稱查找值
let statusValue = StatusCode.Ok; // 200

// 用值反方向查找名稱
let statusName = StatusCode[200]; // "Ok"

```

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block">關於 const Enum</span> </div>

---

<div class="font-bold my-auto  mx-auto text-left p-3 text-[#2e79c7] text-[26px]">總結以上</div>

<ul class="space-y-5 mt-10 text-xl text-[#696969]">
  <li>
  使用 Enum 列舉時，定義的內容須符合 『類型共通性』及 『元素獨特性』
  </li>
  <li>
  Enum 列舉 具有 『反向性查找』功能，可藉由『常數值』來反查『常數值的名稱』
  </li>
  <li>
  使用 const Enum 宣告型別時，會失去『反向取值』功能，好處可減少最終生成的 JavaScript 程式碼
  </li>
</ul>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告: <br/>明文型別 Literal Type
</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
