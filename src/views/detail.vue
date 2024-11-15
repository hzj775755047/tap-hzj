<template>
  <div class="detail">
    <el-row>
      <el-col :span="4">
        <navHome />
      </el-col>
      <el-col :span="24"> 
        <topBar ></topBar>
        <el-row class="lunboPaper">
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
            <el-row  class="imgBox borderBox">
                    <el-col :span="4">
                      <img src="@/assets/img/application/application.jpg" alt="" class="appImg" style="margin-top: 5px;">
                    </el-col>
                    <el-col :span="12" style="text-align: left;padding-left:10px">
                      <div class="mt10 imgTitle">库比利亚</div>
                      <div class="mt10 imgRank">9.3</div>
                      <div class="mt10 imgTag">角色扮演</div>
                    </el-col>
                    <el-col :span="4" style="text-align: center;padding-top: 30px;height: 100px;">
                      <el-button type="success" style="width: 150px;">下 载</el-button>
                    </el-col>
                    <div style="text-align: left;padding-left: 10px;padding-bottom: 10px;">
                        The first Soul Land open-world MMORPG, a classic IP with official authorization. -Preregister now to receive the Southeast Asia exclusive mount - Golden Cup Luo Sanpao,and get a chance to win generous physical prizes! -Explore the limitless
                      </div>
                  </el-row>
                  <el-tabs v-model="activeName" type="border-card" style="text-align: center;">
                    <el-tab-pane label="热门" name="first">
                      <div v-for="o in 10" :key="o" class="text item ">
                        <img src="@/assets/img/application/application.jpg" alt="" class="carouselImg">
                        <div style="text-align: left;padding-left: 10px;padding-bottom: 10px;">
                          The first Soul Land open-world MMORPG, a classic IP with official authorization. -Preregister now to receive the Southeast Asia exclusive mount - Golden Cup Luo Sanpao,and get a chance to win generous physical prizes! -Explore the limitless
                        </div>
                      </div>
                    </el-tab-pane>
                    <el-tab-pane label="最新" name="second">
                      <div v-for="o in 10" :key="o" class="text item ">
                        <img src="@/assets/img/application/c-2.jpg" alt="" class="carouselImg">
                        <div style="text-align: left;padding-left: 10px;padding-bottom: 10px;">
                          The first Soul Land open-world MMORPG, a classic IP with official authorization. -Preregister now to receive the Southeast Asia exclusive mount - Golden Cup Luo Sanpao,and get a chance to win generous physical prizes! -Explore the limitless
                        </div>
                      </div>
                    </el-tab-pane>
                   
                  </el-tabs>

          </el-col>
          <el-col :span="6" style="border-left: 1px solid rgba(0, 0, 0,0.3);margin-top: 70px;">
            <el-card shadow="never" style="border:none;background:rgb(243, 244, 245);border-bottom: 1px solid rgba(0, 0, 0,0.5);text-align: left;" class="rigBG">
              <h4>公告</h4>
              <div class='fontInonce' style="margin-top:20px" >11月 14, 2024</div>
              <div class='fontInonce'>Android版本將於11月 14, 2024正式上線。</div>
              <div class='fontInonce' style="margin-top:20px">11月 14, 2024</div>
              <div class='fontInonce'>Android版本封測玩家招募將於11月 11, 2024開始。 Open-world pocket monster tamer by Tencent! CBT recruitment starts now!</div>
            </el-card>
            
            <div  style="text-align: left;background:rgb(243, 244, 245)">
              相关游戏
              <div v-for="o in 50" :key="o" class="text item" >
                  <el-row :gutter="20" class="imgBox" >
                    <el-col :span="6">
                      <img src="@/assets/img/application/application.jpg" alt="" class="appImg">
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


        <el-row class="lunboMobile" style="display: none;">
          <el-col :span="24">
            <el-card class="carousel" shadow="never">
              <el-row :gutter="20">
                <el-col :span="24">
                <img src="@/assets/img/application/application.jpg" alt="" class="carouselImg">
                <el-row class="carouseDesc">
                  <el-row>
                    <el-col :span="21" style="font-size: 26px;">Real-time combat RPG that intersectsy!</el-col>
                    <el-col :span="2">
                    <div style="font-size: 26px;">TapTap</div>
                    <div style="font-size: 32px;padding-left: 10px;">9.2</div>
                  </el-col>
                  </el-row>
                </el-row>
              </el-col>
              
              </el-row>
              

            </el-card>
            <el-row  class="imgBox borderBox">
                    <el-col :span="4">
                      <img src="@/assets/img/application/application.jpg" alt="" class="appImg" style="margin-top: 5px;">
                    </el-col>
                    <el-col :span="12" style="text-align: left;padding-left:40px">
                      <div class="mt10 imgTitle">库比利亚</div>
                      <div class="mt10 imgRank">9.3</div>
                      <div class="mt10 imgTag">角色扮演</div>
                    </el-col>
                    <el-col :span="8" style="text-align: center;padding-top: 30px;height: 100px;">
                      <el-button type="success" style="width: 100px;">下 载</el-button>
                    </el-col>
                    <div style="text-align: left;padding-left: 10px;padding-bottom: 10px;">
                        The first Soul Land open-world MMORPG, a classic IP with official authorization. -Preregister now to receive the Southeast Asia exclusive mount - Golden Cup Luo Sanpao,and get a chance to win generous physical prizes! -Explore the limitless
                      </div>
                  </el-row>
                  <el-tabs v-model="activeName" type="border-card" style="text-align: center;">
                    <el-tab-pane label="热门" name="first">
                      <div v-for="o in 3" :key="o" class="text item ">
                        <img src="@/assets/img/application/application.jpg" alt="" class="carouselImg">
                        <div style="text-align: left;padding-left: 10px;padding-bottom: 10px;">
                          The first Soul Land open-world MMORPG, a classic IP with official authorization. -Preregister now to receive the Southeast Asia exclusive mount - Golden Cup Luo Sanpao,and get a chance to win generous physical prizes! -Explore the limitless
                        </div>
                      </div>
                    </el-tab-pane>
                    <el-tab-pane label="最新" name="second">
                      <div v-for="o in 3" :key="o" class="text item ">
                        <img src="@/assets/img/application/c-2.jpg" alt="" class="carouselImg">
                        <div style="text-align: left;padding-left: 10px;padding-bottom: 10px;">
                          The first Soul Land open-world MMORPG, a classic IP with official authorization. -Preregister now to receive the Southeast Asia exclusive mount - Golden Cup Luo Sanpao,and get a chance to win generous physical prizes! -Explore the limitless
                        </div>
                      </div>
                    </el-tab-pane>
                   
                  </el-tabs>

          </el-col>
          <el-col :span="24" style="border-left: 1px solid rgba(0, 0, 0,0.3);margin-top: 10px;">
            <el-card shadow="never" style="border:none;background:rgb(243, 244, 245);border-bottom: 1px solid rgba(0, 0, 0,0.5);text-align: left;" class="rigBG">
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
                    <el-col :span="6">
                      <img src="@/assets/img/application/application.jpg" alt="" class="appImg">
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
      activeName:'first'
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
@media only screen and (max-width: 600px) {
  .detail{

    border-left: none !important;
  }
}
.detail{
  width: 70%;
  margin-left: 30%;
  border-left: 1px solid  rgba(0, 0, 0, 0.3);
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
      /* border-radius: 20px; */
    }
    .appImg{
      width:80px;
      height:80px;
      border-radius: 20px;
      margin-left: 10px;
    }
    .imgTitle{
      font-weight: bold;
    }
    .imgBox{
      /* margin-top: 10px; */
      /* border: 1px solid rgba(0, 0, 0, 0.3); */
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
    .borderBox{
      border-top: 1px solid  rgba(0, 0, 0, 0.3);
      border-bottom: 1px solid  rgba(0, 0, 0, 0.3);
    }

</style>
