<template>
  <div class="content">
    商家详情内容{{id}}
  </div>
</template>

<script>
// import axios from 'axios'
// import Info from '@/components/Info'

export default {
  layout: 'merchant',
  computed: {
    id() {
      return this.$nuxt.$route.params.id
    }
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
</style>
