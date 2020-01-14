<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <strong>{{fun()}}</strong>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  methods:{
    fun:function(){
        let str="a,b,c,d,e,f"
        let s=str.substring(0,str.lastIndexOf(','));
        return s;
    }
  },
  components: {
    HelloWorld
  }
}
</script>
