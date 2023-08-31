<template>
    <header>
      <div class="content-left">
        <img src="~/assets/logo.png" />
      </div>

      <div class="content-center">
        <ul>
          <li><NuxtLink to="/home">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/pricing">Pricing</NuxtLink></li>
          <li><NuxtLink to="/contact">Contact</NuxtLink></li>  
        </ul>
      </div>

      <div class="content-rigth">
        <button class="button-log"><NuxtLink to="/login">Login</NuxtLink></button>
        <button><NuxtLink to="/register">Register</NuxtLink></button> 
      </div>
    </header>
</template>



<script lang="ts" setup>

</script>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Zen+Maru+Gothic&display=swap');

  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-family: 'Zen Maru Gothic';
    font-size: 1.1rem;
    color: #031F49;
    
  }
  header .content-left {
    width: 10rem;
  }

  header .content-left img{
    width: 100%;
  }

  header .content-center {
    width: 33%;
  }
  header .content-center ul {
    display: flex;
    justify-content: space-between; 
  }

  header .content-center ul li, a {
    text-decoration: none;
    list-style: none;
    color: inherit;
    &:hover{
      color: #0a76c2;
    }
  }

  header .content-center ul li a::after {
      content: '';
      display: block;
      width: 0;
      height: 2px;
      background: rgb(250, 98, 64);
      transition: width .3s;
  }

  header .content-center ul li a:hover::after {
    width: 100%;
    }

  header .content-rigth {
    margin-right: 2rem;
  }

  header .content-rigth button {
    background-color: transparent;
    border: 1px solid;
    padding: 0.5rem 2rem;
    border-radius: 2rem;
    font-family: 'Zen Maru Gothic';
    font-size: 1.1rem;
    &:hover {
      background-color: #f8f8f8;
    }
  }

  header .content-rigth .button-log {
    margin-right: 2rem;
  }

</style>