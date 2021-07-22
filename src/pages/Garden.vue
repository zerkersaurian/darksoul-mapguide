<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/castle')">Lothric Castle</a>
      <a class="symbol">&nbsp; , &nbsp; </a>
      <a class="location" @click="goTo('/highwall')">High Wall of Lothric</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Consumed King's Garden</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/graves')">Untended Graves</a>
    </div>
    
    <g-image class="map1" src="~/picture/Garden/1.jpg"/>

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