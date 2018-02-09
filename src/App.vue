<template>
  <div id="app">
    <div class="picture-box">
      <picture-zoom :img-url="imgUrl" :scale="scale"></picture-zoom>
    </div>
  </div>
</template>

<script>
import PictureZoom from './components/picture-zoom'

export default {
  name: 'App',
  components: {
    'picture-zoom': PictureZoom
  },
  data () {
    return {
      imgUrl : '../static/imgDemo.jpg',
      scale: 4
    }
  }
}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.picture-box{
  width: 500px;
  height: 300px;
  border: 1px #eee solid;
}
</style>
