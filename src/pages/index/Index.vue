<template>
	<div>
	  <index-header />
	  <index-swiper />
	</div>
  
</template>

<script>
import HeaderComponent from './Header';
import SwiperComponent from './Swiper';

export default {
  components:{
    "index-header":HeaderComponent,
    "index-swiper":SwiperComponent
  }
}
</script>

<style scoped>

</style>
