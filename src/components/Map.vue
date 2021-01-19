<template>
  <div class="map">
    <h1 class="header">SIMETRA offices</h1>
    <mapbox
      access-token="pk.eyJ1IjoidGhuZHItIiwiYSI6ImNrazQyOW00MzAycnAydW82OGZncnB0Y3gifQ.pFE4VjgJRUPlIOSCCj8ENg"
      :map-options="{
        style: 'mapbox://styles/mapbox/light-v9',
        center: [-96, 37.8],
        zoom: 3
      }"
    />
  </div>
</template>

<script>
import Mapbox from 'mapbox-gl-vue'

export default {
  components: { Mapbox },
  name: 'Map'
}
</script>

<style lang="sass" scoped>
h1
  font-size: 2rem
#map
  position: absolute
  top: 0
  right: 0
  left: 0
  bottom: 0
  height: 100vh
  width: 100%
  z-index: 1
.header
  z-index: 2
  width: 100%
  position: absolute
</style>
