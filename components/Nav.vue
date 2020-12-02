<template>
 

     
      <!-- Center Navigation -->
      <nav class="container">
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
      </nav>
  
 

</template>

<script>


export default {

  data() {
    return {
      links: [
          { slug: '1', name: '首页', href: '/' },
          { slug: '2', name: '建材信息', href: '/material' },
          { slug: '3', name: '招采信息', href: '/zhaocai' },
          { slug: '4', name: '我需要', href: '/needAndGive/need' },
          { slug: '5', name: '我提供', href: '/needAndGive/give' },
          { slug: '6', name: '建筑社区', href: 'https:baidu.com' },
          { slug: '7', name: '找工作', href: '/job' },
      ]
    }
  },
 

}
</script>

<style scoped>
.container {
    height: 50px;
    border: 1px solid #ccc;
    margin-bottom: 10px;
}
ul {
    overflow: hidden;
}
li {
    float: left;
    margin: 5px;
}
</style>
