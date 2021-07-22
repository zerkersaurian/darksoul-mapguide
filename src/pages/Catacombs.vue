<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/farron')">Farron Keep</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Catacombs of Carthus</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/lake')">Smouldering lake</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/valley')">Irithyll of the Boreal Valley</a>
    </div>
    
    <g-image class="map1" src="~/picture/Catacomb/1.jpg"/>
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