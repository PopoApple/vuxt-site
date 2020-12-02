<template>
  <header class="header">
      header
      <div @click="$router.push('/')">
        logo
      </div>
      
      <a href="/history">浏览记录</a>
      <el-button @click="$router.push('/searchResult/material')">搜索</el-button>
      <el-button v-if="btnInfo" class="btn" @click="$router.push(btnInfo.path)">{{ btnInfo.name }}</el-button>
  </header>
</template>

<script>
// import NuxtLogo from '~/assets/images/logo.svg?inline'
const btnInfoArry = [
  {path: '/publishGoods', name: '发布商品', forPaths: ['/material/merchant']},
  {path: '/publishJob', name: '发布职位', forPaths: [ /\/job(\/\*)*/]},
  {path: '/publishNeed', name: '发布需求信息', forPaths: [ '/needAndGive/need', '/publishNeed', /\/needDetail(\/\*)*/]},
  {path: '/publishGive', name: '发布供应信息', forPaths: [ '/needAndGive/give', '/publishGive', /\/giveDetail(\/\*)*/]}
]
export default {
  computed: {
    btnInfo() {
      let path = this.$nuxt.$route.path
      for (let i = 0; i < btnInfoArry.length; i++) {
        let bi = btnInfoArry[i]
        if (bi.forPaths.findIndex(d => {
          return (typeof d === 'string' && d === path) || (typeof d === 'object' && d.test(path))
        }) >= 0) {
          return bi
        }
      }
      return null
    }
  }
  // components: {
  //   NuxtLogo
  // },
  // data() {
  //   return {
  //     onTop: true
  //   }
  // },
  // mounted() {
  //   window.addEventListener('scroll', this.handleScroll)
  // },
  // destroyed() {
  //   window.removeEventListener('scroll', this.handleScroll)
  // },
  // methods: {
  //   handleScroll() {
  //     this.onTop = window.pageYOffset < 60
  //   }
  // }
}
</script>
<style scoped>
.header {
  position: relative;
  height: 100px;
  border: 1px solid #ccc;
  margin-bottom: 10px;
}
.btn {
  position: absolute;
  right: 10px;
  bottom: 10px;
}
</style>
