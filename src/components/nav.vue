<template>
  <div class="nav">
    <div @click="toHome" class="icon-i">
      <img src="@/assets/img/taptap.png" alt="" class="imgi">
    </div>
    <div class="mt50">
      <img class="item-icon" src="@/assets/img/tabbar/home.svg" alt="">
      <!-- <img slot="item-icon-active" src="@/assets/img/tabbar/home_active.svg" alt=""> -->
      <span class="item-text">游戏</span>
    </div>
    <div class="mt30">
      <img class="item-icon" src="@/assets/img/tabbar/category.svg" alt="">
      <!-- <img slot="item-icon-active" src="@/assets/img/tabbar/home_active.svg" alt=""> -->
      <span class="item-text">设定</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navHome',
  props: {
    msg: String
  },
  components: {},
  data(){
    return {
     
    }
  },
  computed: {
    noMore(){
    }
  },
  created(){
  },
  methods: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.home{
  width: 70%;
  margin: auto;
}
.nav{
  
position:fixed;
left: 400px;
}
.imgi{
  width: 150px;
  
}
.item-icon{
  position: relative;
  width: 40px;
  top: 10px;
}
.item-text{
  display: inline-block;
  margin-left: 20px;
  line-height: 32px;
  font-size: 32px;
}
</style>
