<template>
  <div id="app">
    
    <!-- header -->
      <!-- logo -->
      <!-- nav-link -->
    <MyHeader/>
  



    <!-- main -->

      <!-- sez -->
        <!-- comp. x3 -->
        <!-- comp. x3 -->
      <!-- /sez -->

      <!-- ask -->

      <!-- sez -->
        <!-- comp. x18 -->
      <!-- /sez -->

      <!-- cit. -->

      <!-- sez -->
        <!-- comp. x3 -->
      <!-- /sez -->

      <!-- Enquiry -->

    <!-- footer -->
    
    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'

export default {
  name: 'App',
  components: {
    MyHeader
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Helvetica, Arial, sans-serif;
}
</style>
