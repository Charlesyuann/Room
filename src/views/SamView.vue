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
            <button onclick="rose1()" class="btn btn-outline-success" type="button">Search</button>
          </div>
        </div>
    </nav>
      <layoutheader/>
      <layoutTwice/>
    </div>
  </template>
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
        }
      }
    }
  </script>
  <style>
  .SELECT{
      display: flex;
      width: 100%;
  }
  .slide{
      width: 1200px;
      height: 720px;
  }
  .peace{
      display: flex;
      width: 100%;
  }
  .card{
      width: 28%;
      margin: 0 2%;
  }
  .card:hover{
      cursor: pointer;
      border-color: darkred;border-style: solid;
  }
  .pagination{
      margin-top: 20px;

  }
  /* .btn_area .son{
      width: 100px;
      height: 50px;
      border-color: darkred;border-style: solid;
      background-color: firebrick;color:white;
      transition: 0.5s ease-in;
  }
  .btn_area .son:hover{
      box-shadow: inset 100px 0 0 0 green;
      color: violet; 
      cursor: pointer;
  } */
  .navbar-light .navbar-brand{
      font-family: fantasy;
      font-weight: 700;color: brown;
  }
  .loku2{
      width: 400x;
      height: 360px;
  }
  .join{
    width: 180px;
    margin-right: 40px;
  }
  .title{
    font-size: 40px;
  }
</style>
  