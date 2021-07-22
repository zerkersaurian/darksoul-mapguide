<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/firelink')">Firelink Shrine</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">High wall of Lothric</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/undead')">Undead Settlement</a>
    </div>
    
    <g-image class="map1" src="~/picture/Highwall/1.jpg"/>
    <g-image class="map2" src="~/picture/Highwall/2.jpg"/>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Ceremetry of Ash'
  },
  methods: {
    goTo: function(string){
       this.$router.push(string); 
    }
  },
}
</script>