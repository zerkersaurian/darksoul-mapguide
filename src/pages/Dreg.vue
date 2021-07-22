<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/kiln')">Kiln of the First Flame</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/painted')">Painted World of Ariandel</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">The Dreg Heap</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/ringed')">The Ringed City</a>
    </div>
    
    <g-image class="map1" src="~/picture/Dreg/1.jpg"/>
    <g-image class="map1" src="~/picture/Dreg/2.jpg"/>
    <g-image class="map1" src="~/picture/Dreg/3.jpg"/>
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