<template>
  <div>
    <div class="left box">
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
    </div>
    <div class="right box">
        <nuxt-child />
    </div>
  </div>
</template>

<script>
// import axios from 'axios'
// import Info from '@/components/Info'

export default {
  layout: 'simple',
  meta: {
    name: '用户中心'
  },
    data() {
    return {
      links: [
          { slug: '1', name: '我的发布', href: '/userCenter/publish' },
          { slug: '2', name: '我要发布', href: '/userCenter/wantPublish' },
          { slug: '3', name: '我的关注', href: '/userCenter/myFocus' },
          { slug: '4', name: '我的收藏', href: '/userCenter/myCollection' },
          { slug: '5', name: '我的意向承接', href: '/userCenter/wantGet' },
          { slug: '6', name: '我的评论', href: '/userCenter/wantPublish' },
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
.left {
    width: 100px;
    float: left;
}
.right {
    margin-left: 110px;
}
</style>
