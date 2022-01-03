<template>
  <b-container fluid class="wrapper">
    
    <div class="aside"><Aside /></div>
    
    <b-container fluid class="main">
      
      <div class="header"><Header/></div>
      
      <div class="content">
        <Nuxt/>
      </div>
      
    
    </b-container>
  </b-container>
</template>


<script>
import Aside from '@/components/main/Aside'
import Header from '@/components/main/Header'
import Footer from '@/components/main/Footer'

export default {
  components: {Aside, Header, Footer}
}
</script>


<style lang="css" scoped>
  .wrapper {
    display: flex;
  }
  
  .header {
    background-color: aqua;
  }
</style>