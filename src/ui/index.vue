<template>
  <div>
     <fieldset>
         <legend>lcy的组件封装test1</legend>
         <h1>lcy</h1>
          <h2>123</h2>
          <slot></slot>
     </fieldset>
  </div>
</template>

<script>
export default {
  name: 'zjtest1',
  data(){
      return{
          msg:"第一次封装"
      }
  },
  props:{
      tel:{
         type:Number,
         dafault:() =>{
             return 123456
         }
      }
  }
}
</script>

<style scoped>
</style>
