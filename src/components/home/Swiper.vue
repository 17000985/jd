<template>
  <div class="swiper">
    <van-swipe :autoplay="2000">
      <van-swipe-item v-for="(image, index) in images" :key="index">
     <img v-lazy="image" fit="contain" />
    </van-swipe-item>
</van-swipe>

  </div>
</template>

<script type="text/javascript">
export default {
  name:"swiper",
  data() {
    return {
       images: [
        'https://m.360buyimg.com/mobilecms/s700x280_jfs/t1/139195/35/7338/49569/5f4cc151E0501ff9a/4a5994f6d00e339c.jpg!cr_1125x445_0_171!q70.jpg.dpg',
        'https://m.360buyimg.com/mobilecms/s700x280_jfs/t1/119535/6/15287/131076/5f4cbd4cE3c6bfbec/d214abe541e98d3f.jpg!cr_1125x445_0_171!q70.jpg.dpg',
        'https://m.360buyimg.com/mobilecms/s700x280_jfs/t1/128067/4/10158/85966/5f3e6352Ebc10ea41/13d196f6fb00270c.jpg!cr_1125x445_0_171!q70.jpg.dpg',
        'https://m.360buyimg.com/mobilecms/s700x280_jfs/t1/126157/33/10714/73723/5f43272aE11ef4ce8/efde1c885d078813.jpg!cr_1125x445_0_171!q70.jpg.dpg',
        'https://m.360buyimg.com/mobilecms/s700x280_jfs/t1/128315/14/10190/87640/5f3e70a7E331f3a92/75b16a93d947e448.jpg!cr_1125x445_0_171!q70.jpg.dpg',
        'https://m.360buyimg.com/mobilecms/s700x280_jfs/t1/148730/16/5847/84520/5f3e6fcdEa67a7227/9149b63a9216c7ad.jpg!cr_1125x445_0_171!q70.jpg.dpg'
        ],
    }
  },
  components: {

  }
}
</script>

<style>
.swiper{
    display: flex;
    justify-content:center;
    margin-top: 54px;
    margin-bottom: 40px;
    width: 100%;
    height: 100px;
    background-color: #C82519;
    border-radius: 0 0 5% 5%;
}
.van-swipe{
    border-radius: 6px 6px 6px 6px;
    height: 140px;
    width: 94%;
    

}

  .swiper .van-swipe-item img{
      height: 100%;
      width: 100%;
  }
</style>
