<template>
  <div>
    <div class="list">
      <a class="list-item" href="/needAndGive/need/1">
        需求信息1
      </a>
      <a class="list-item" href="/needAndGive/need/2">
        需求信息2
      </a>
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
.filter {
  height: 200px;
  border: 1px solid #ccc;
  margin-bottom: 10px;
}
.list-item {
  height: 50px;
  border: 1px solid #ccc;
  margin-bottom: 10px;
  display: block;
}
</style>
