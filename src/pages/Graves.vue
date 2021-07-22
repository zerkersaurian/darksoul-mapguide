<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/garden')">Consumed King's Garden</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Untended Graves</a>
    </div>
    
    <g-image class="map1" src="~/picture/Grave/1.jpg"/>

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