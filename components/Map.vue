<template>
  <div id="mapid"></div>
</template>
<script>
export default {
  name: 'Map',
  data: () => ({}),
  mounted() {
    let L
    const mymap = L.map('mapid').setView([51.505, -0.09], 13)

  },
}
</script>

<style scoped>
#mapid {
  height: 65vh;
}
</style>
