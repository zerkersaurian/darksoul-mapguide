<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/road')">Road of Sacrifices</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Cathedral of the Deep</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/farron')">Farron Keep</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/painted')">Painted World of Ariandel</a>
    </div>
    
    <g-image class="map1" src="~/picture/Cathedral/1.jpg"/>
    <g-image class="map2" src="~/picture/Cathedral/2.jpg"/>
    <g-image class="map2" src="~/picture/Cathedral/3.jpg"/>
    <g-image class="map2" src="~/picture/Cathedral/4.jpg"/>
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