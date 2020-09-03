<template>
<div>
  <div class="seckill">
    <div class="sk1">京东秒杀</div>
    <div class="sk2">
        <div class="sk">
        <div class="sk21">16点场</div>
        <div class="sk22">00:00:00</div>
        </div>
    </div>
    <div class="sk3">更多秒杀></div>
    
   
  </div>
  <van-tabs v-model="active" swipeable>
  <van-tab v-for="index in 15" :title="'选项 ' + index">
    内容 {{ index }}
  </van-tab>
</van-tabs>
  </div>
</template>

<script type="text/javascript">
export default {
  name:"seckill",
  data() {
    return {

    }
  },
  components: {

  }
}
</script>

<style>
.seckill{
display: flex;
justify-content:left;
margin: auto;
width: 94%;
background-color: #fff;
font-size: .9rem;
color: #333;
}
.seckill .sk1{
margin-right: 0.2rem;
}
.seckill .sk2{
flex:2;
align-self:left;


}
.seckill .sk2 .sk{
 border-radius: 4rem;
 border: 1px solid #f10001;
 width: 7.5rem;
 display: flex;
}
.seckill .sk2 .sk21{
    font-size: 0.7rem;
    text-align: center;
    border-radius: 4rem;
    line-height: 1.4;
    color: #fff;
    width: 4rem;
    background-image: linear-gradient(90deg,#f10001,#fe4e18);
     
}
.seckill .sk2 .sk22{
    width: 5rem;
    text-align: right;
    margin-right: 0.5rem;
    color: #fe4e18;
    border-radius: 4rem;
}
.seckill .sk3{
flex:1;
text-align: right;
font-size: 0.8rem;
color: rgb(242, 48, 48);;
}
</style>
