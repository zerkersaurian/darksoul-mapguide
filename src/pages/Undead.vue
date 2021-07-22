<template>
  <Layout>
    <div class="location-linking">
      <a class="location" @click="goTo('/highwall')">Highwall of Lothric</a>
      <a class="symbol">&nbsp; << &nbsp; </a>
      <a class="location-this">Undead Settlement</a>
      <a class="symbol">&nbsp; >> &nbsp; </a>
      <a class="location" @click="goTo('/road')">Road of Sacrifices</a>
    </div>
    
    <g-image class="map1" src="~/picture/Undead/1.jpg"/>
    <g-image class="map2" src="~/picture/Undead/2.jpg"/>
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