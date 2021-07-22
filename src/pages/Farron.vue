<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/road')">Road of Sacrifices</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Farron Keep</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/catacombs')">Catacombs of Carthus</a>
    </div>
    
    <g-image class="map1" src="~/picture/Farron/1.jpg"/>
    <g-image class="map2" src="~/picture/Farron/2.jpg"/>
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