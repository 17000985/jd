<template>
    <van-tabbar v-model="active" active-color="#D81E06" inactive-color="#8A8A8A" border route>
      <van-tabbar-item  replace to="/home">
        <span>首页</span>
        <template #icon="props">
        <img :src="props.active ? icon1.active : icon1.inactive" />
        </template>
      </van-tabbar-item>
      <van-tabbar-item  icon="category" replace to="/classify">
        <span>分类</span>
        <template #icon="props">
        <img :src="props.active ? icon2.active : icon2.inactive" />
        </template>
      </van-tabbar-item>
      <van-tabbar-item  icon="friends-o" replace to="/jingxi">京喜</van-tabbar-item>
      <van-tabbar-item   replace to="/cart">
        <span>购物车</span>
        <template #icon="props">
        <img :src="props.active ? icon4.active : icon4.inactive" />
        </template>
      </van-tabbar-item>
      <van-tabbar-item  replace to="/me">
        <span>未登录</span>
        <template #icon="props">
        <img :src="props.active ? icon5.active : icon5.inactive" />
        </template>
      </van-tabbar-item>
    </van-tabbar>
</template>

<script type="text/javascript">
export default {
  name:"tabbar",
  data() {
    return {
      active: 0,    
        icon1: {
          active: require('../assets/tabbar/home2.svg'),
          inactive: require('../assets/tabbar/home1.svg'),
        },
        icon2: {
          active: require('../assets/tabbar/category2.svg'),
          inactive:require('../assets/tabbar/category1.svg'),
        },
         icon3: {
          active: require('../assets/tabbar/category2.svg'),
          inactive:require('../assets/tabbar/category1.svg'),
        },
         icon4: {
          active: require('../assets/tabbar/cart2.svg'),
          inactive:require('../assets/tabbar/cart1.svg'),
        },
         icon5: {
          active: require('../assets/tabbar/me2.svg'),
          inactive:require('../assets/tabbar/me1.svg'),
        }
          
    }
   }
  
}
</script>

<style>
.van-tabbar{
   box-shadow: 0 0 10px 0 hsla(0,6%,58%,.6);
} 
</style>
