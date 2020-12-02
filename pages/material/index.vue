<template>
  <div class="wrap">
    <div class="carousel">
      轮播图
    </div>
    <div class="cata">
      分类
    </div>
    <div class="login">
      登录
    </div>
    <div class="content">
      建材首页
    </div>
  </div>
</template>

<script>
// import axios from 'axios'
// import Info from '@/components/Info'

export default {
//   components: {
//     Info,
//   },
//   asyncData ({ params }) {
//     return new Promise((res) => {
//       setTimeout(() => {
//         res( { info: 'xxxxx' })
//       }, 3000)
//     })
//  },
//  data() {
//    return { title: '哈哈哈' }
//  }
}
</script>

<style scoped>
.wrap {
  position: relative;
}
.carousel{
    margin: 0 310px 10px 210px;
  border: 1px solid #ccc;
  height: 300px;
}
.cata{
  position: absolute;
  top: -60px;
  left: 0;
  width: 200px;
  height: 360px;
  margin: 0 auto 10px;
  border: 1px solid #ccc;
}
.login{
  position: absolute;
  top: -60px;
  right: 0;
  width: 300px;
  height: 360px;
  margin: 0 auto 10px;
  border: 1px solid #ccc;
}
.content {
  height: 600px;
  border: 1px solid #ccc;
  margin-bottom: 10px;
}
</style>
