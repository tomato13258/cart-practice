<script></script>
<template>
    <div class="w-[250px] h-[550px] bg-slate-500  rounded-[5px]">
        <img src="https://fakeimg.pl/250x250/000000,100/f7c995,200" class="mb-[10px]">
        <div class="item-text-box px-[10px]">
          <div class=" text-[28px] font-bold text-neutral-200 mb-[10px]">我是商品</div>
          <div class=" text-[14px] text-neutral-300 mb-[50px]">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been  </div>
          <div class="text-[#f7c995] mb-[20px] font-bold">＄400 NT</div>
          <!--按鈕組 -->
          <div class="">
            <div class="flex justify-start mb-[5px]">
              <button class="itemBtn itemBtn-l w-[30px] h-[30px] bg-slate-800 flex items-center justify-center text-white">-</button>
              <div class="bg-gray-100 w-full  h-[30px] text-[20px] text-center">1</div>
              <button class="itemBtn itemBtn-r w-[30px] h-[30px] bg-slate-800 flex items-center justify-center text-white">+</button>
            </div>
            <button class="add-cart w-[100%] h-[30px] bg-slate-800 flex items-center justify-center text-white text-[16px] rounded-[5px]">加入購物車</button>
          </div>
        </div>
      </div>
</template>

<style scoped>
.itemBtn,.add-cart{
  transition:  .3s;
}
.itemBtn:hover,.add-cart:hover{
  background-color: #c98333;
 
}
.itemBtn-l{
  border-radius: 5px 0 0 5px;
}
.itemBtn-r{
  border-radius: 0 5px 5px 0;
}
</style>