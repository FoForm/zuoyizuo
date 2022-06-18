<template>
  <div id="app">
    <ul>
      <li v-for="item in add" :key="item">{{item}}</li>
    </ul>
    <button @click="box">走一走</button>
  </div>
  
</template>

<script>
  export default{
    name:"add",
    data () {
      return {
        add:["帅哥","美女","程序员"]
      }
    },
    methods:{
      box(){
        this.add.push(this.add[0])
        this.add.shift()
      }
    }
  }
</script>

<style>

</style>
