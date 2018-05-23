<template>
  <div id="app">
    <First />
    <Second />
    <Third />
    <Fourth />
    <Fifth />
    <FooterBlock />
  </div>
</template>

<script>
import First from './components/FirstBlock.vue'
import Second from './components/SecondBlock.vue'
import Third from './components/ThirdBlock.vue'
import Fourth from './components/FourthBlock.vue'
import Fifth from './components/FifthBlock.vue'
import FooterBlock from './components/FooterBlock.vue'

import Firebase from './components/Firebase.vue'

export default {
  name: 'app',
  components: {
    First,
    Second,
    Third,
    Fourth,
    Fifth,
    FooterBlock,
    Firebase
  }
}
</script>

<style scoped>
#app{
  height: 100%;
  width: 100%;
}
</style>

