<template>
    <div class="Sam">
        <nav class="navbar navbar-light bg-light">
          <div class="container-fluid">
            <a class="navbar-brand title">Wine</a>
            <div class="d-flex">
              <!-- <button class="btn btn-outline-info join" onclick="javascript:window.location.href='wineRegister.html'">Join Us</button>  -->
              <!-- <button class="btn btn-outline-info join" onclick="javascript:window.location.href='wineRegister.html'">Login</button> -->
              <button class="btn btn-outline-info join" @click="goLogin()">Login</button> 
              <input id="rose" type="text" class="form-control me-2"  placeholder="Search" >
              <button @click="rose1()" class="btn btn-outline-success" type="button">Search</button>
            </div>
          </div>
        </nav>
      <layoutheader/>
      <p class="verse1"><b>BASIC</b></p>
      <layoutTwice/>
    </div>
  </template>13
<script>
  import layoutheader from '@/components/layoutHeader.vue'
  import layoutTwice from '@/components/layoutTwice.vue'

  export default {
    name: 'SamView',
    components: {
      layoutTwice,
      layoutheader
  },
    methods: {
      goLogin () {
        this.$router.push('/')
      },
      rose1() {
        this.$router.push('/')  
      }
    }
  }
</script>
<style>
  .verse1{
    margin-top: 30px;
  }
</style>
