<template>
  <Layout>
    <div class="location-linking">
      <a class="location-this">Ceremetry Of Ash</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/firelink')">Firelink Shrine</a>
    </div>
    
    <g-image class="map1" src="~/picture/Ceremetry/1.png"/>
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