<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/catacombs')">Catacombs of Carthus</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Smouldering lake</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/valley')">Irithyll of the Boreal Valley</a>
    </div>
    
    <g-image class="map1" src="~/picture/Lake/1.jpg"/>
    <g-image class="map1" src="~/picture/Lake/2.jpg"/>
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