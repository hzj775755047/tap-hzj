<template>
  <div class="home">
    <el-row>
      <el-col :span="4">
        <navHome />
      </el-col>
      <el-col :span="24"> 
        <topBar ></topBar>
        <el-row>
          <el-col :span="12">
            <el-card class="carousel" shadow="never">
              <el-row :gutter="20">
                <el-col :span="24">
                <img src="@/assets/img/application/application.jpg" alt="" class="carouselImg">
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
              <el-col :span="6"  v-for="o in 4" :key="o" class="text item" style="margin-top: -100px;">
                  <el-row :gutter="20" class="imgBox">
                    <el-col :span="24">
                      <img src="@/assets/img/application/application.jpg" alt="" class="carouselRightImg">
                    </el-col>
                    
                  </el-row>
              </el-col>
              </el-row>
              

            </el-card>
            <el-row :gutter="20" class="imgBox">
                    <el-col :span="10">
                      <img src="@/assets/img/application/application.jpg" alt="" class="carouselRightImg">
                    </el-col>
                    <el-col :span="6" style="text-align: left;">
                      <div class="mt10 imgTitle">库比利亚</div>
                      <div class="mt10 imgRank">9.3</div>
                      <div class="mt10 imgTag">角色扮演</div>
                    </el-col>
                    <el-col :span="8" style="text-align: center;padding-top: 30px;">
                      <el-button type="success" style="width: 150px;">下 载</el-button>
                    </el-col>
                  </el-row>
          </el-col>
          <el-col :span="6">
            <el-card shadow="never" style="border:none;background:rgb(243, 244, 245);border-bottom: 1px solid rgba(0, 0, 0,0.5);" class="rigBG">
              <h4>公告</h4>
              <div class='fontInonce' style="margin-top:20px" >11月 14, 2024</div>
              <div class='fontInonce'>Android版本將於11月 14, 2024正式上線。</div>
              <div class='fontInonce' style="margin-top:20px">11月 14, 2024</div>
              <div class='fontInonce'>Android版本封測玩家招募將於11月 11, 2024開始。 Open-world pocket monster tamer by Tencent! CBT recruitment starts now!</div>
            </el-card>
            
            <div  style="text-align: left;background:rgb(243, 244, 245)">
              相关游戏
              <div v-for="o in 10" :key="o" class="text item" >
                  <el-row :gutter="20" class="imgBox" >
                    <el-col :span="10">
                      <img src="@/assets/img/application/application.jpg" alt="" class="carouselRightImg">
                    </el-col>
                    <el-col :span="14">
                      <div class="mt10 imgTitle">库比利亚</div>
                      <div class="mt10 imgRank">9.3</div>
                      <div class="mt10 imgTag">角色扮演</div>
                    </el-col>
                  </el-row>
                </div>
            </div>
          </el-col>
        </el-row>

       
      </el-col>
    </el-row>
  </div>
</template>

<script>
import navHome from '@/components/nav1.vue'
import topBar from '@/components/topBar1.vue'
export default {
  name: 'detail',
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
    margin-top: 70px;
    height:620px;
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
      margin-top: 10px;
      border: 1px solid rgba(0, 0, 0, 0.3);
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
