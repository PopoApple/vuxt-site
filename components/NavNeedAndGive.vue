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
          { slug: '1', name: '我需要', href: '/needAndGive/need' },
          { slug: '2', name: '我提供', href: '/needAndGive/give' },
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
