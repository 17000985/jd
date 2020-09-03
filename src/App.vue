<template>
  <div id="app">
    <router-view />
    <tabbar/>


 
  </div>
</template>
<script>
import tabbar from './components/TabBar'
export default {
  data() {
    return {
      
    }
  },
  components:{
     tabbar
  }

}
</script>

<style>

</style>
