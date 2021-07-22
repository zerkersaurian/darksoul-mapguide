<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/ceremetry')">Cemetery of Ash</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Firelink Shrine</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/highwall')">High Wall of Lothric</a>
    </div>
    
    <g-image class="map1" src="~/picture/Firelink/1.jpg"/>
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