<script>
// import returnBtn from '@/components/returnBtn.vue';
// import cartItemCard from '@/components/cartItemCard.vue'


export default {
  components: {
    // returnBtn,
    // cartItemCard,

  },
  data() {
    return {
      returnValue: true,

    }
  },
  emits: ['returnClick'],
  methods: {
    // 回傳值給父層
    returnClick() {
      this.$emit('returnClick', this.returnValue);
      console.log(this.returnValue);
    },
  },
};
</script>


<template>
  <main class="w-full bg-neutral-200 px-[8%] py-[5%]  ">
    <span class="ml-[150px]">購買完成!</span>

    <div class="items-box  flex justify-around  flex-wrap mb-[80px] ">
      
      <!-- 這裏面放商品卡 -->
      <div class="w-[80%] h-[150px] bg-slate-500  flex ">
        <img src="https://fakeimg.pl/150x150/000000,100/f7c995,200" class="">
        <div class="item-text-box   px-[10px] flex items-center">
          <div class="font-bold text-neutral-200 px-[50px]">我是商品</div>

          <!--按鈕組 -->
          <div class="">
            <div class="flex justify-start px-[50px]">
              <div class=" text-[#f7c995] w-full  h-[30px] text-[20px] text-center px-[50px]">1</div>
            </div>

          </div>
          <div class="text-[#f7c995] px-[50px] font-bold">＄400 NT</div>
        </div>

      </div>

    </div>
    <div class=" w-full  ">
      <div class="bg-slate-500">
        <div class="ml-[150px]">
          <span>購買人資訊:</span>
          <div class="mb-[10px]">
            <span class="">姓名:</span>
            <input type="text">
          </div>
          <div class="mb-[10px]">
            <span class="">電話:</span>
            <input type="tel">
          </div>
          <div class="mb-[10px]">
            <span class="">地址:</span>
            <input type="text">
          </div>
          <div class="mb-[10px]">
            <span class="">信箱:</span>
            <input type="e-mail">
          </div>
          <div class="">
            <span>付款方式:</span>
            <input type="radio" name="pay" id="pay1">
            <label for="pay1">信用卡</label>
            <input type="radio" name="pay" id="pay2">
            <label for="pay2">貨到付款</label>
          </div>
          <div class="">
            <span>運送方式:</span>
            <input type="radio" name="deliver" id="deliver1">
            <label for="deliver1">宅配</label>
            <input type="radio" name="deliver" id="deliver2">
            <label for="deliver2">超商取貨</label>
          </div>
        </div>
      </div>
    </div>



    <div class="flex justify-around">
      <router-link to="/">回首頁</router-link>
    </div>
  </main>
</template>

<style scoped></style>