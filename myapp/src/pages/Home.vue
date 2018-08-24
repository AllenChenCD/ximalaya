<template>
    <div>    
        <Swiper></Swiper> 
        <div class="hot">
          热门推荐
        </div>
        <div class=" ">
            <ul>
              <li v-for="(item,index) in datas" :key="index">
                <a href="">
                  {{item.name}}
                </a>
              </li>
            </ul>
        </div>
    </div>        
</template>

<script>
import Swiper from "components/swiper";
import {tuijian} from "data/tuijian"


export default {
  name: "home",
  data(){
    return {
      datas:[]
    }
  },
  components: {
    Swiper
  },
  created(){
    console.log(tuijian)
    console.log(tuijian.award.AdditionalData.TdkData.data.tdkMeta.quickEntries)
    this.datas = tuijian.award.AdditionalData.TdkData.data.tdkMeta.quickEntries

  
  }
};
</script>

<style>
.hot{
  text-align: center;
  color: brown;
  font-size: 18px;
  font-weight: 700;
  margin: 20px
}


</style>
