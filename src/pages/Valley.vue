<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/catacombs')">Catacombs of Carthus</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Irithyll of the Boreal Valley</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/dungeon')">Irithyll Dungeon</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/castle')">Lothric Castle</a>
    </div>
    
    <g-image class="map1" src="~/picture/Valley/1.jpg"/>
    <g-image class="map1" src="~/picture/Valley/2.jpg"/>
    <g-image class="map1" src="~/picture/Valley/3.jpg"/>
    <g-image class="map1" src="~/picture/Valley/4.jpg"/>

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