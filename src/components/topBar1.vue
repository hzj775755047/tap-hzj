<template>
  <div class="topBar">
      <!-- 搜索框 -->
      <div class="search1" style="font-size: 22px;">
        详细信息
      </div>
      <!-- login -->
      <div class="login-img" >
        <input class="search-input" v-model="searchStr" type="text" placeholder="搜索" />
        <img  src="@/assets/img/index/default.png" alt="" class="searchImg">
      </div>
    </div>
</template>

<script>
export default {
  name: 'topBar1',
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
.search1{
    width:40%;
    display: inline-block;
    
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
    width: 400px;
    margin-right: 200px;
    cursor: pointer;
  }
  .login-img .searchImg{
    position: relative;
    top:10px;
    margin-left: 10px;
    width: 40px;
  }
  .searchLogo{
    position: relative;
    top:10px;
    width:100px;
    height:40px;
  }
</style>
