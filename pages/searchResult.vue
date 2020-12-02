<template>
  <div>
    
        <ul>
          <li
            v-for="link in links"
            :key="link.slug"
          >
            <a
              :key="link.href"
              :href="link.href"
             
            >
              {{ link.name }}
          
            </a>
          </li>
        </ul>
  

        <nuxt-child />
   
  </div>
</template>

<script>
// import axios from 'axios'
// import Info from '@/components/Info'

export default {
    data() {
    return {
      links: [
          { slug: '1', name: '建材', href: '/searchResult/material' },
          { slug: '2', name: '招采', href: '/searchResult/zhaocai' },
          { slug: '3', name: '社区', href: '/searchResult/shequ' },
          { slug: '4', name: '需求', href: '/searchResult/need' },
          { slug: '5', name: '提供', href: '/searchResult/give' },
          { slug: '6', name: '工作', href: '/searchResult/job' },
      ]
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
.box {
  height: 800px;
  border: 1px solid #ccc;
}
ul {
  overflow: hidden;
}
li {
  float: left;
  margin: 10px;
}

</style>
