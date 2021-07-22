<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/valley')">Irithyll of the Boreal Valley</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Anor Londo</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/dungeon')">Irithyll Dungeon</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/castle')">Lothric Castle</a>
    </div>
    
    <g-image class="map1" src="~/picture/AnorLondo/1.jpg"/>

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