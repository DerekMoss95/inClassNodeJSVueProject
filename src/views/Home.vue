<template>
  <div class="home">
    <HelloWorld msg="Hello"/>
    <h1>This is a home page</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>
