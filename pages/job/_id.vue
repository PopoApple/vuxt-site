<template>
  <div class="content">
    职位详情{{id}}
    <a href="/merchantDetail/1">公司介绍</a>
  </div>
</template>

<script>
// import axios from 'axios'
// import Info from '@/components/Info'

export default {
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
