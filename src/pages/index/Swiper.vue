<!-- The ref attr used to find the swiper instance -->
<template>
  <swiper :options="swiperOption" ref="mySwiper">

    <swiper-slide>
    	<div class="index-swiper-con">
    		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1710/f5/57137c621d75ba02.jpg_640x200_b984ddf7.jpg"/>
    	</div>
    </swiper-slide>
   
    <swiper-slide>
    	<div class="index-swiper-con">
    		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1609/15/630b82d932a3c402.jpg_640x200_862e836b.jpg"/>
    	</div>
    </swiper-slide>

     <swiper-slide>
     	<div class="index-swiper-con">
     		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1711/5a/cb4a0ccffeb99b02.jpg_640x200_1b0b75b1.jpg"/>
     	</div>
     </swiper-slide>

     <swiper-slide>
     	<div class="index-swiper-con">
     		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1711/aa/4f6639ef6473c002.jpg_640x200_7806eb33.jpg"/>
     	</div>
     </swiper-slide>

     <swiper-slide>
     	 <div class="index-swiper-con">
    	 	<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1712/af/faa87a138c7a4802.jpg_640x200_6f54d29a.jpg"/>
     	 </div>
     </swiper-slide>

     <swiper-slide>
     	<div class="index-swiper-con">
   	 		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1712/c2/3004f2d4a022d002.jpg_640x200_5ed9f26c.jpg"/>
     	</div>
     </swiper-slide>

     <swiper-slide>
     	<div class="index-swiper-con">
     		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1712/5c/723bbb93e9683f02.jpg_640x200_7d38c6ad.jpg"/>
     	</div>
     </swiper-slide>

     <swiper-slide>
     	<div class="index-swiper-con">
     		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1712/2d/1f9a9776d9e9d102.jpg_640x200_38cdba53.jpg"/>
     	</div>
     </swiper-slide>

     <swiper-slide>
     	<div class="index-swiper-con">
     		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1712/cc/150da60866ee4602.jpg_640x200_a5bf772c.jpg"/>
     	</div>
     </swiper-slide>

     <swiper-slide>
     	<div class="index-swiper-con">
     		<img class="index-swiper-img" src="http://img1.qunarzz.com/piao/fusion/1711/cd/5ff8869f365e7e02.jpg_640x200_097b1798.jpg"/>
     	</div>
     </swiper-slide>

    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
</template>

<script>
  import { swiper, swiperSlide } from 'vue-awesome-swiper'

  export default {
    name: 'carrousel',
    data() {
      return {
        swiperOption: {
          autoplay:3000,
          direction:'horizontal',
          autoHeight:true,
          pagination:'.swiper-pagination',
          observeParents:true,
        }
      }
    },
   
    mounted() {
      this.$refs.mySwiper.swiper.slideTo(3, 1000, false)
    },
    components: {
	   swiper,
	   swiperSlide
	}
  }
</script>

<style scoped>
.index-swiper-con {
	overflow:hidden;
	width:100%;
	height:0;
	padding-bottom:31.25%
}

.index-swiper-img {
	width:100%;
}
</style>