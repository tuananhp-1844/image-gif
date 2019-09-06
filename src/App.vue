<template>
  <div id="app">
    <HelloWorld 
      image = "https://scontent.fhan2-4.fna.fbcdn.net/v/t39.1997-6/p240x240/68120606_410165212934465_9210642140336488448_n.png?_nc_cat=104&_nc_eui2=AeHkfXPNV-1cS5XtMrZ-LsWFbFSmQPplPv3FxWGVJr0Z19ZmL57tMvRrKFgmFUiujUCKuA1fk1iDrSWVu1OZ9hBIWULxs9_QKX_pXFTsUI2E-Q&_nc_oc=AQmBajqdmXeJ3QSZlSl_GYMu-xcuKu8aloKxGnMZM9pkshwyD6CW3OszB5yURriBnu0&_nc_ht=scontent.fhan2-4.fna&oh=f39b12ff10d2ffa84218d8958c8ab14d&oe=5E0A40E0"
      :width="100"
      :height="100"
      :column="4"
      :row="3"
      :max="10"
      :frame="1"
    />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
