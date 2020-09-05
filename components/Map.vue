<template>
  <div id="mapid"></div>
</template>
<script>
export default {
  name: 'Map',
  data: () => ({}),
  mounted() {
    //   eslint-disable-next-line
    const mymap = L.map('mapid').setView([6.465422, 3.406448], 10)
    //   eslint-disable-next-line
    L.tileLayer(
      'https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token={accessToken}',
      {
        attribution:
          'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors, <a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, Imagery © <a href="https://www.mapbox.com/">Mapbox</a>',
        maxZoom: 18,
        id: 'mapbox/streets-v11',
        tileSize: 512,
        zoomOffset: -1,
        accessToken:
          'pk.eyJ1IjoiZ3JheWNvbGR3YXRlciIsImEiOiJja2VxYWZsOXQyZXJsMnhwaTJtcGVyc3BkIn0.OaxshyP_7MU5RVD4jrA7vQ',
      }
    ).addTo(mymap)
  },
}
</script>

<style scoped>
#mapid {
  height: 65vh;
}
</style>
