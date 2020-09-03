<template>
  <div class="grid">
    <van-grid :column-num="5" :border=false icon-size="40px">
    <van-grid-item v-for="(val,key) in list" :key="key" :icon="val.icon" :text="val.name" />
    </van-grid>
  </div>
</template>

<script type="text/javascript">
export default {
  name:"grid",
  data() {
    return {
       list:[
           {name:'京东超市',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/125678/35/5947/4868/5efbf28cEbf04a25a/e2bcc411170524f0.png.webp'},
           {name:'数码电器',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/135931/4/3281/5598/5efbf2c0Edbdc82c7/ed9861b4ddfb9f30.png.webp'},
           {name:'京东服饰',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/140012/8/1804/3641/5efbf318E38bd5dad/0db99d859ab16ce9.png.webp'},
           {name:'京东生鲜',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/129215/21/5978/3618/5efbf344Ebec23ae8/59712d986b10bb0a.png.webp'},
           {name:'京东到家',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/116602/7/11200/3796/5efbf375Ebba41029/f07cc166f368fa05.png.webp'},
           {name:'充值缴费',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/146390/3/1846/4909/5efbf39aEe5f5f797/300071558a9ab078.png.webp'},
           {name:'9.9元拼',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/143365/25/1824/3716/5efbf3c0E5175e1fb/88f6227257a29f1d.png.webp'},
           {name:'领劵',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/113589/24/11332/4897/5efbf3feE705d87db/e5c12d5e943266b9.png.webp'},
           {name:'领金贴',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/131663/33/3380/3674/5efbf50fEf79cf314/af4b57d2383e605d.png.webp'},
           {name:'PLUS会员',icon:'https://m.360buyimg.com/mobilecms/s120x120_jfs/t1/123730/37/5924/4189/5efbf567E0a226121/d04df7c74c87cf68.png.webp'},
           ]
    }
  }
  
}
</script>

<style>
.van-grid-item .van-grid-item__content{
    background-color: #F6F6F6;
}
</style>
