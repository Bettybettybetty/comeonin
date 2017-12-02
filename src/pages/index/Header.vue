<template>
  <div class="index_header">   
    <div class="index_header_left iconfont icon-back"></div>
    <div class="index_header_center">
      <div class="index_header_center_icon iconfont icon-fangdajing">
        <div class="index_header_center_content">输入城市/景点/游玩主题</div>
      </div>
    </div>
    <div class="index_header_right">北京</div>
    
  </div>
</template>

<script>
export default {
 
}
</script>


<style scoped>
.index_header{
  position:relative;
  height:.88rem;
  background:#00bcd4;
}
.index_header_left{
  float:left;
  width:.4rem;
  padding:0 .2rem;
  line-height:.88rem;
  font-size:.4rem;
  color:#fff;
}

.index_header_center {
  position:absolute;
  left:.8rem;
  right:1.28rem;
  top:.14rem;
  line-height:.6rem;
  background:#fff;
  border-radius:.06rem;
  text-indent:.1rem;
  color:#ccc;
}
.index_header_center_icon {
  display:inline-block;
}

.index_header_center_content {
  display:inline-block;
}

.index_header_right {
  float:right;
  width:1.28rem;
  line-height:.88rem;
  text-align:center;
  color:#fff;
  white-space:nowrap;
  overflow:hidden;
  text-overflow:ellipsis;

}

.index_header_right::after {
  content : "\0020";
  border: .1rem solid transparent;
  border-top: .1rem solid #fff;
  position: absolute;
  top:.4rem;
  right:0;
  margin-right:.1rem;
}



</style>
