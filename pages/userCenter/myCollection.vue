<template>
  <div class="wrap">
   我的收藏
  </div>
</template>

<script>
// import axios from 'axios'
// import Info from '@/components/Info'

export default {
  meta: {
    name: '我的收藏'
  },
  created() {
    console.log( this.$nuxt.$route)
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
</style>
