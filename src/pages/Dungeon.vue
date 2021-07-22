<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/valley')">Irithyll of the Boreal Valley</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Irithyll Dungeon</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/profaned')">Profaned Capital</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/peak')">Archdragon Peak</a>
    </div>
    
    <g-image class="map1" src="~/picture/Dungeon/1.jpg"/>
    <g-image class="map1" src="~/picture/Dungeon/2.jpg"/>

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