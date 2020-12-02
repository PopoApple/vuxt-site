<template>
 <div>
        {{ info }}
      </div>
</template>

<script>

import axios from 'axios'
export default {
  data() {
    return {
      info: null
    }
  },
  created() {
    setTimeout(() => {
        this.info = '哈哈哈22'
      }, 5000)
  },
  // asyncData ({ params }) {
  //   return new Promise((res) => {
  //     setTimeout(() => {
  //       res( { info: '哈哈哈22' })
  //     }, 8000)
  //   })
    // return axios.get('https://api.github.com/users/PopoApple')
    //   .then((res) => {
    //     console.log(res)
    //     return { info: res.data.login }
    //   })
 //},
}
</script>
