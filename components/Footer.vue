<template>
    <footer>
      <div class="content-left">
        <ul>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/policy">Policy</NuxtLink></li>
          <li><NuxtLink to="/terms">Terms</NuxtLink></li> 
        </ul>
      </div>

      <div class="content-center">
        <div>
          <img src="~/assets/dark-logo.png" />
        </div>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
      </div>

      <div class="content-right">
        <ul>
          <li><NuxtLink to="/contact">Contact</NuxtLink></li>
        </ul>
      </div>

    </footer>
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Zen+Maru+Gothic&display=swap');

  footer {
    border: solid;
    display: flex;
    justify-content: space-between;
    background-color: #031F49;
    color: #FFFFFF;
    font-family: 'Zen Maru Gothic';
    position: absolute;
    right: 0;
    bottom: 0;
    left: 0;
  }

  footer .content-left {
    width: 33%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  footer li{
    list-style: none;
    color: inherit;
  }
  footer  li a {
    text-decoration: none;
    color: inherit;
    &:hover {
      color: #9eb6c7;
    }
  }
  footer .content-center {
    width: 33%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 2rem;
    justify-content: center;
  }
  footer .content-center div {
    width: 7rem;
  }

  footer .content-center div img{
    width: 100%;
  }

  footer .content-right {
    width: 33%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  ul {
    padding: 0;
  }



</style>