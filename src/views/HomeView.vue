<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
  <form-comp/>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import FormComp from '@/components/form-comp.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    FormComp
  }
}
</script>
