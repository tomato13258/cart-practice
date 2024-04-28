<script>
import itemCard from '@/components/itemCard.vue'
import itemCard2 from '@/components/itemCard-2.vue'
import switchNtns from '@/components/switch-ntns.vue'
export default {

  components: {
    switchNtns,
    itemCard,
    itemCard2,

  },
};

// import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <switchNtns />
  <main class="w-full bg-neutral-200 px-[8%] py-[5%] ">
    
    <div class="items-box  flex justify-around gap-[20px]  gap-y-[50px] flex-wrap ">
      <!-- 這裏面放商品卡 -->
      <itemCard />
      <itemCard2 />
    </div>
  </main>


</template>

<style scoped>
.itemBtn,
.add-cart {
  transition: .3s;
}

.itemBtn:hover,
.add-cart:hover {
  background-color: #c98333;

}
</style>
