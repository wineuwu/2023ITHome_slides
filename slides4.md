---
class: text-[#2e79c7]
highlighter: shiki
lineNumbers: false
colorSchema: "light"
transition: slide-left
title: day4
---

<div class="flex h-full space-x-8 mb-10  text-[#2e79c7] justify-center items-center">
  <div class="font-bold  text-left tracking-wide p-3  text-[35px] relative">在 <span class="text-center p-0.5  px-3  text-[55px] inline-block"> 大腦升級 </span> 後  <br>我想要學 TypeScript 了  
  <span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-70 block"> TSConfig 常見基本設定</span> 
  </div>
  <div class="h-42 w-42">
    <img src ="/tslogo.png" class="mx-auto"/>
  </div>
</div>
<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold my-auto mx-auto  text-center p-3 text-[#2e79c7] text-3xl leading-12">今日的內容</div>

<ul class="mt-10 text-xl text-[#2e79c7]">
 
  <li> 常見 CompilerOption 設定 </li>
  <li> 其他常見設定 </li>
  <li> 注意事項 </li>
  
</ul>

---

<div class="font-bold  text-left mb-5 tracking-wide  text-[#2e79c7] text-[26px] relative"> 
前情提要: 
</div>

<div class="flex  space-x-30 h-150px mt-20 text-center w-auto pt-10 justify-center relative"><div class="bg-[#f1f1f1] h-20 text-center leading-20  w-20 inline-block">index.ts</div>
<div class=" border-t m-auto top-20 right-0 left-0 w-70% -z-1 absolute"></div>
  <div class="bg-[#f1f1f1] h-20 text-center py-6 w-20 inline-block">tsc</div>
  <div class="bg-[#2e79c7] h-20 text-center text-white  py-6 w-40 inline-block">tsconfig.json</div>
  <div class="bg-[#f1f1f1] h-20 text-center py-6 w-20 inline-block">index.js</div>
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold  text-left mb-5 tracking-wide  text-[#2e79c7] text-[26px] relative"> 
建立 TS Config 
</div>

<span class="font-bold bg-[#2e79c7] text-white text-center p-1 w-34 block">command line</span>

<div class="mt-10" >

```
tsc --init

```

<span class="font-bold bg-[#2e79c7] my-10 text-white text-center p-1 w-50 block">手動建立 tsconfig.json</span>

```
// tsconfig.json

{}

```

<div class="rounded-sm bg-[#FFECEC80] my-10 p-4 text-[#CE0000] text-[14px]">
注意事項 : 如果是手動建立，tsconfig.json檔案不可以是空白，最起碼要給一個 {}
</div>

</div>

---

<div class="rounded-full m-auto bg-[#CEDCEC66] h-70  text-center  top-0 right-0  bottom-0 left-0 w-70 -z-3 absolute " ></div>
<div class="font-bold mx-auto  mt-50  text-center text-24px  text-[#2F6FB0]    " >
  CompilerOptions <br>常見基礎設定
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="rounded-full m-auto bg-[#CEDCEC66] h-70  text-center  top-0 right-0  bottom-0 left-0 w-70 -z-3 absolute " ></div>
<div class="font-bold mx-auto  mt-55  text-center text-24px  text-[#2F6FB0]    " >
  其他常見設定
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class=" space-y-4 text-[#2e79c7]">
  <div class="font-bold text-left mb-10  tracking-wide text-[#2e79c7] text-[26px] relative"> 注意事項
  </div>
  <div class="space-y-5 mt-20">
  <div >
   1. files 不能使用 『glob模式』方式去指定 『多個資料夾』或『多個檔案』；
  </div>
  <div>
   2. 宣告於 files 中的檔案即使有匹配到 exclude 指定檔名，還是會被編譯
  </div>

  <div>
   3. 編譯的優先權為  files > exclude > include
  </div>

  </div>
  
</div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>

---

<div class="font-bold   mx-auto mt-40 text-center p-3 text-[#2e79c7] text-3xl"><span class="bg-[#2e79c7] mt-8 text-white text-center p-1 text-[20px] w-80 inline-block"> 下集預告: <br/>TS型別類型 - 原始資料型別</span> </div>

<div class="mx-auto bg-[#2e79c7] h-3 right-0 bottom-0 left-0 absolute"></div>
