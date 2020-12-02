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
          { slug: '1', name: '首页', href: '/material' },
          { slug: '2', name: '商品', href: '/material/goods' },
          { slug: '3', name: '商家', href: '/material/merchant' },
      ]
    }
  },
 

}
</script>

<style scoped>
.container {
        height: 50px;
    border: 1px solid #ccc;
    margin: 0 310px 10px 210px;
}
ul {
    overflow: hidden;
}
li {
    float: left;
    margin: 5px;
}
</style>
