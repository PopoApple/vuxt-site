<template>
  <div>
    <Nav/>
    <div class="content">
      首页
      <div class="carousel" @click="$router.push('/article/1')">轮播图</div>
      <Login/>
      <a href="/oneImg">一张图</a>
    </div>
  </div>
</template>

<script>
// import axios from 'axios'
// import Info from '@/components/Info'

export default {
  meta: {
    name: '首页'
  },
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
.content {
  height: 800px;
  border: 1px solid #ccc;
  margin-bottom: 10px;
}
.carousel {
  border: 1px solid #ccc;
  height: 300px;
  width: 500px;
  margin: 10px auto;
}
</style>
