<template>
  <div class="home">
    <el-row>
      <el-col :span="4">
        <navHome />
      </el-col>
      <el-col :span="24"> 
        <topBar ></topBar>
        <div class="homeContent">
          <div>
            精选游戏
            <el-card class="carousel" shadow="never">
              <el-row :gutter="20"class="lunboPaper">
                <el-col :span="18" >
                  <img src="@/assets/img/application/application.jpg" alt="" class="carouselImg" @click="toDetail">
                  <el-row class="carouseDesc">
                    <el-row>
                      <el-col :span="21" style="font-size: 26px;">Real-time combat RPG that intersects multiple worlds! Official launchtoday!</el-col>
                      <el-col :span="2">
                      <div style="font-size: 26px;">TapTap</div>
                      <div style="font-size: 32px;padding-left: 10px;">9.2</div>
                    </el-col>
                    </el-row>
                  </el-row>
                </el-col>
                <el-col :span="6" >
                  <div v-for="o in 4" :key="o" class="text item">
                    <el-row :gutter="20" class="imgBox">
                      <el-col :span="10">
                        <img src="@/assets/img/application/application.jpg" alt="" class="carouselRightImg" @click="toDetail">
                      </el-col>
                      <el-col :span="14">
                        <div class="mt10 imgTitle">库比利亚</div>
                        <div class="mt10 imgRank">9.3</div>
                        <div class="mt10 imgTag">角色扮演</div>
                      </el-col>
                    </el-row>
                  </div>
                </el-col>
              </el-row>
              <el-row :gutter="20"class="lunboMobile" style="display: none;">
                <el-col :span="24" >
                <img src="@/assets/img/application/application.jpg" alt="" class="carouselImg" @click="toDetail">
                <el-row class="carouseDesc">
                  <el-row>
                    <el-col :span="21" style="font-size: 26px;">Real-time combat RPG that intersects multiple worlds! Official launchtoday!</el-col>
                    <el-col :span="2">
                    <div style="font-size: 26px;">TapTap</div>
                    <div style="font-size: 32px;padding-left: 10px;">9.2</div>
                  </el-col>
                  </el-row>
                </el-row>
              </el-col>
              
              </el-row>
            </el-card>
          </div>
          <div>
            热门游戏和话题
            <el-row :gutter="20" class="lunboPaper">
              <el-col :span="8" v-for="o in 10" :key="o" class="mt10">
                <div>
                  <img src="@/assets/img/application/application.jpg" alt="" class="imgList" @click="toDetail">
                </div>
                  <div class="mt10 imgTitle">库比利亚</div>
                      <div class="mt10 imgTag">角色扮演</div>
                      <div class="mt10 imgDesc">本週最受「浪漫」遊戲玩家喜爱的遊戲</div>
              </el-col>
            </el-row>
            <el-row :gutter="20" class="lunboMobile" style="display: none;">
              <el-col :span="24" v-for="o in 10" :key="o" class="mt10">
                <div>
                  <img src="@/assets/img/application/application.jpg" alt="" class="imgList" @click="toDetail"> 
                </div>
                  <div class="mt10 imgTitle">库比利亚</div>
                      <div class="mt10 imgTag">角色扮演</div>
                      <div class="mt10 imgDesc">本週最受「浪漫」遊戲玩家喜爱的遊戲</div>
              </el-col>
            </el-row>
          </div>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import navHome from '@/components/nav.vue'
import topBar from '@/components/topBar.vue'
export default {
  name: 'home',
  props: {
    msg: String
  },
  components: {navHome,topBar},
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
    toDetail(){
      this.$router.push("/detail");
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.home{
  width: 70%;
  margin-left: 30%;
}
.homeContent{
  margin-top: 50px;
  text-align: left;
  }
  .carousel{
    margin-top: 20px;
    height:500px;
    border-radius: 20px;
    background-color: #f5f7f8;

  }
  .carouselImg{
      width: 100%;
      height: 470px;
      border-radius: 20px;
    }
    .carouselRightImg{
      width: 100%;
      height: 100px;
      border-radius: 20px;
    }
    .imgTitle{
      font-weight: bold;
    }
    .imgBox{
      border: 1px solid #000;
      border-radius: 20px;
      margin-top: 10px;
    }
    .carouseDesc{
      padding-top: 20px;
      padding-left: 30px;
      position: relative;
      width: 100%;
      color:#fff;
      top:-105px;
      height:100px;
      border-bottom-left-radius: 20px;
      background-color: rgba(0, 0, 0, 0.3);
      border-bottom-right-radius: 20px;
    }
    .imgList{
      width: 100%;
      border-radius: 10px;
      height: 200px;
    }
</style>
