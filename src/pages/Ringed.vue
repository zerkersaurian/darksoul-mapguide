<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/dreg')">The Dreg Heap</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">The Ringed City</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/painted')">Painted World of Ariandel</a>
    </div>
    
    <g-image class="map1" src="~/picture/RingedCity/1.jpg"/>
    <g-image class="map1" src="~/picture/RingedCity/2.jpg"/>
    <g-image class="map1" src="~/picture/RingedCity/3.jpg"/>
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