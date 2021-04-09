<template>
  <div class="home">
    <button @click="getHandle">发送get请求</button>
      <button @click="postHandle">发送post请求</button>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import axios from "axios";
export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  methods:{
    getHandle(){
      axios.get("https://api.cat-shop.penkuoer.com/api/v1/products",{
        params:{
          page:3,
          per:2
        },
        headers:{}
      })
      .then(res =>console.log(res))
    },
   getHandle(){
      axios.get("https://api.cat-shop.penkuoer.com/api/v1/products",{
        params:{
          page:3,
          per:2
        },
        headers:{}
      })
      .then(res =>console.log(res))
    }
}
}
</script>
