<template>
  <div class="navbar">
    <van-search
       show-action
       placeholder="| 请输入搜索关键词"
       shape="round"
       background="#C82519"
       :left-icon="icon"
    >
    <template #left>
    <div @click="classify"><img src="../../assets/navbar/more.svg" alt=""></div>
    </template>
    <template #action>
    <div style="color:white">登录</div>
    </template>
</van-search>
  </div>
</template>

<script type="text/javascript">
export default {
  name:"navbar",
  data() {
    return {
       icon:require('../../assets/navbar/jd.png')
    }
  },
  methods:{
    classify(){
      console.log(1);
      this.$router.push({path:'/classify'})
    }
  }
}
</script>

<style>
.navbar{
  position: fixed;
  top:0;
  left: 0;
  right: 0;
  z-index: 2;
  
}
.navbar img{
    width: 20px;
    height: 25px;
    margin-right: 8px;

}
.navbar .van-icon{
    width: 20px;
    height: 20px;
    margin-right: 5px;
}

</style>
