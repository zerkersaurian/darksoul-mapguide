<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/castle')">Lothric Castle</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Grand Archives</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/kiln')">Kiln of the First Flame</a>
    </div>
    
    <g-image class="map1" src="~/picture/Archive/1.jpg"/>
    <g-image class="map1" src="~/picture/Archive/2.jpg"/>
    <g-image class="map1" src="~/picture/Archive/3.jpg"/>

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