<template>
  <div class="topBar">
      <!-- 搜索框 -->
      <div @click="toHome" class="icon-i" style="display: none;">
        <img src="@/assets/img/taptap.png" alt="" class="imgi">
      </div>
      <div class="search">
        <img class="search-icon" src="@/assets/img/index/search.svg" alt="" >
        <input class="search-input" v-model="searchStr" type="text" placeholder="搜索" />
      </div>
      <!-- login -->
      <div class="login-img" >
        <img  src="@/assets/img/application/2222.png" alt="" class="searchLogo">
        <img  src="@/assets/img/index/default.png" alt="" class="searchImg">
      </div>
      <div>
        <div class="mobileNav" style="display: none;">
          <img class="item-icon" src="@/assets/img/tabbar/home.svg" alt="">
          <!-- <img slot="item-icon-active" src="@/assets/img/tabbar/home_active.svg" alt=""> -->
          <span class="item-text">游戏</span>
        </div>
        <div class="mobileNav"  style="display: none;">
          <img class="item-icon" src="@/assets/img/tabbar/category.svg" alt="">
          <!-- <img slot="item-icon-active" src="@/assets/img/tabbar/home_active.svg" alt=""> -->
          <span class="item-text">设定</span>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'topBar',
  props: {
    msg: String
  },
  components: {},
  data(){
    return {
      searchStr:'',
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

.topBar{
  position: fixed;
  width: 100%;
  background-color: #fff;
  top: 0;
  text-align: left;
  height: 80px;
  padding-top: 20px;
  z-index:99;
}
.search{
    width:50%;
    display: inline-block;
    padding-left: 10%;
    
  }
  .search-icon{
    width: 24px;
    cursor: pointer;
  }
  .search-input{
    border: none;
    margin-left: 8px;
    padding-left: 20px;
    height: 30px;
    width: 50%;
    border-radius: 50px;
    background-color: #dae6ec;
  }
  .login-img{
    display: inline-block;
    margin-left: 10px;
    width: 200px;
    margin-right: 200px;
    cursor: pointer;
  }
  .login-img .searchImg{
    position: relative;
    top:10px;
    width: 40px;
  }
  .searchLogo{
    position: relative;
    top:10px;
    width:100px;
    height:40px;
  }
</style>
