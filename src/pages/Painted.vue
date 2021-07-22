<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/cathedral')">Cathedral of the Deep</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Painted World of Ariandel</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/dreg')">The Dreg Heap</a>
    </div>
    
    <g-image class="map1" src="~/picture/PaintedWorld/1.jpg"/>
    <g-image class="map1" src="~/picture/PaintedWorld/2.jpg"/>
    <g-image class="map1" src="~/picture/PaintedWorld/3.jpg"/>
    <g-image class="map1" src="~/picture/PaintedWorld/4.jpg"/>

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