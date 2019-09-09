<template>
  <div id="app">
    <HelloWorld 
      image = "https://scontent.fhan5-6.fna.fbcdn.net/v/t39.1997-6/s526x395/47421285_2005256322890945_2278943500189827072_n.png?_nc_cat=105&_nc_oc=AQnLigbk94_Mo0GFULiZ-vOPI-lrL-WwawHyLqKYsKRgw5j4aVjPrbZss0ePh3rK7gA&_nc_ht=scontent.fhan5-6.fna&oh=e635b2529d098303c2e5746952f8d846&oe=5E15F158"
      :width="100"
      :height="100"
      :column="6"
      :row="5"
      :max="30"
      :frame="10"
      :loop="7"
    />
    <HelloWorld 
      image = "https://miro.medium.com/max/3072/1*WhDjw8GiV5o0flBXM4LXEw.png"
      :width="100"
      :height="100"
      :column="6"
      :row="1"
      :max="6"
      :frame="10"
      :loop="7"
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
