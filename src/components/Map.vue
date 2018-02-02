<script>
export default {
  name: "maps",
  data () {
    return {
        markers: [{
          position: {lat: -33.4406159, lng: -70.6603104}
        }],
        mapStyle: {
            styles:[{"featureType":"administrative","elementType":"labels.text.fill","stylers":[{"color":"#444444"}]},{"featureType":"landscape","elementType":"all","stylers":[{"color":"#ffffff"}]},{"featureType":"landscape","elementType":"labels","stylers":[{"visibility":"off"}]},{"featureType":"poi","elementType":"all","stylers":[{"visibility":"on"},{"color":"#e9f3f2"}]},{"featureType":"poi","elementType":"labels","stylers":[{"visibility":"off"}]},{"featureType":"road","elementType":"all","stylers":[{"saturation":-100},{"lightness":45}]},{"featureType":"road","elementType":"geometry","stylers":[{"visibility":"on"},{"color":"#f6f7f8"},{"lightness":"-2"},{"gamma":"1"}]},{"featureType":"road.highway","elementType":"all","stylers":[{"visibility":"simplified"}]},{"featureType":"road.arterial","elementType":"labels.icon","stylers":[{"visibility":"off"}]},{"featureType":"transit","elementType":"all","stylers":[{"visibility":"off"}]},{"featureType":"water","elementType":"all","stylers":[{"color":"#f2f6f8"},{"visibility":"on"}]}]
        }
    }
  }
}
</script>

<template>
    <gmap-map
    :center="{lat:-33.4406159, lng:-70.6603104}"
    :zoom="16"
    map-type-id="terrain"
    v-bind:options="mapStyle"
    style="width: 100%; height: 100%">
        <gmap-marker
            :key="index"
            v-for="(m, index) in markers"
            :position="m.position"
            :clickable="true"
            :draggable="true"
            @click="center=m.position">
        </gmap-marker>
    </gmap-map>
</template>

<style scoped>
    .vue-map-container{
        min-height: 400px;
    }
</style>
