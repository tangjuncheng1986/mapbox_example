<!--
 * @Descripttion:
 * @Author: jiegiser
 * @Date: 2020-03-26 08:05:27
 * @LastEditors: jiegiser
 * @LastEditTime: 2020-03-26 14:42:10
 -->
<template>
  <div id="mapCon" />
</template>

<script>
import mapboxgl from '../mapbox'
export default {
  name: 'HelloWorld',
  mounted() {
    var map = new mapboxgl.Map({
      container: 'mapCon',
      style: 'mapbox://styles/mapbox/streets-v11',
      center: [114.41703647375107, 23.10750961303711],
      zoom: 12
    })
    console.log(map)
  }
}
</script>
<style scoped>
#mapCon {
  height: calc(100vh - 85px);
  width: 100%;
}
.selectInfo {
  position: absolute;
  top: 10px;
  right: 10px;
}
</style>
