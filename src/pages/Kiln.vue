<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/firelink')">Firelink Shrine</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/archives')">Grand Archives</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Kiln of the First Flame</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/dreg')">The Dreg Heap</a>
    </div>
    
    <g-image class="map1" src="~/picture/Kiln/1.jpg"/>
  </Layout>
</template>

<script>
export default {
  methods: {
    goTo: function(string){
       this.$router.push(string); 
    }
  },
}
</script>
