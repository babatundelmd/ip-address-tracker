<template>
  <div class="wrapper">
    <div class="header">this is good</div>
    <Map></Map>
  </div>
</template>

<script>
import Map from '@/components/Map'
export default {
  components: { Map },
}
</script>

<style scoped>
* {
  margin: 0;
  box-sizing: border-box;
}
.header {
  background: url('/images/pattern-bg.png') no-repeat;
  background-size: cover;
  width: 100%;
  height: 35vh;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
