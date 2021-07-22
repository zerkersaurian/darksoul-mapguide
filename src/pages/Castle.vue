<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/highwall')">High Wall of Lothric</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Lohric Castle</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/archives')">Grand Archives</a>
    </div>
    
    <g-image class="map1" src="~/picture/Castle/1.jpg"/>
    <g-image class="map1" src="~/picture/Castle/2.jpg"/>
    <g-image class="map1" src="~/picture/Castle/3.jpg"/>

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