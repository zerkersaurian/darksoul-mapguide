<template>
  <Layout>
    <div>
      <ul class="location_list">
        <li @click="goTo('/ceremetry')"><g-image class="location_img" src="~/picture/index_img/cemetery_of_ash.jpg"/><br>Cemetery of Ash</li>
        <li @click="goTo('/firelink')"><g-image class="location_img" src="~/picture/index_img/firelink_shrine.jpg"/><br>Firelink Shrine</li>
        <li @click="goTo('/highwall')"><g-image class="location_img" src="~/picture/index_img/highwall_of_lothric.jpg"/><br>High Wall of Lothric</li>
        <li @click="goTo('/undead')"><g-image class="location_img" src="~/picture/index_img/undead_settlement.jpg"/><br>Undead Settlement</li>
        <li @click="goTo('/road')"><g-image class="location_img" src="~/picture/index_img/road_of_sacrifice.jpg"/><br>Road of Sacrifices</li>
        <li @click="goTo('/cathedral')"><g-image class="location_img" src="~/picture/index_img/cathedral_of_the_deep.jpg"/><br>Cathedral of the Deep</li>
        <li @click="goTo('/farron')"><g-image class="location_img" src="~/picture/index_img/farron_keep.jpg"/><br>Farron Keep</li>
        <li @click="goTo('/catacombs')"><g-image class="location_img" src="~/picture/index_img/catacombs_of_carthus.jpg"/><br>Catacombs of Carthus</li>
        <li @click="goTo('/lake')"><g-image class="location_img" src="~/picture/index_img/smouldering_lake.jpg"/><br>Smouldering Lake</li>
        <li @click="goTo('/valley')"><g-image class="location_img" src="~/picture/index_img/irithyll_of_the_boreal_valley.jpg"/><br>Irithyll of the Boreal Valley</li>
        <li @click="goTo('/dungeon')"><g-image class="location_img" src="~/picture/index_img/irithyll_dungeon.jpg"/><br>Irithyll Dungeon</li>
        <li @click="goTo('/profaned')"><g-image class="location_img" src="~/picture/index_img/profaned_capital.jpg"/><br>Profaned Capital</li>
        <li @click="goTo('/anor')"><g-image class="location_img" src="~/picture/index_img/anor_londo.jpg"/><br>Anor Londo</li>
        <li @click="goTo('/castle')"><g-image class="location_img" src="~/picture/index_img/lothric_castle.jpg"/><br>Lothric Castle</li>
        <li @click="goTo('/garden')"><g-image class="location_img" src="~/picture/index_img/consumed_king_garden.jpg"/><br>Consumed King's Garden</li>
        <li @click="goTo('/archives')"><g-image class="location_img" src="~/picture/index_img/grand_archives.jpg"/><br>Grand Archives</li>
        <li @click="goTo('/graves')"><g-image class="location_img" src="~/picture/index_img/untended_graves.jpg"/><br>Untended Graves</li>
        <li @click="goTo('/peak')"><g-image class="location_img" src="~/picture/index_img/archdragon_peak.jpg"/><br>Archdragon Peak</li>
        <li @click="goTo('/kiln')"><g-image class="location_img" src="~/picture/index_img/kiln_of_the_first_flame.jpg"/><br>Kiln of the First Flame</li>
        <li @click="goTo('/painted')"><g-image class="location_img" src="~/picture/index_img/painted_world_of_ariandel.jpg"/><br>Painted World of Ariandel</li>
        <li @click="goTo('/dreg')"><g-image class="location_img" src="~/picture/index_img/the_dreg_heap.jpg"/><br>The Dreg Heap</li>
        <li @click="goTo('/ringed')"><g-image class="location_img" src="~/picture/index_img/ringed_city.jpg"/><br>The Ringed City</li>
      </ul>
    </div>
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

<style>
  .symbol{
    font-size: 50px;
    color: orange;
    }
  .location-this{
    text-decoration: underline #D40000;
    transition: 0.3s
  }
  .location-this:hover{
    text-shadow: 1px 1px 8px #FF6600;
    text-decoration: underline #FF5E00;
    transition: 0.3s
  }
  .location-linking{
    margin-top: 20px;
    display:block;
    font-size: 40px;
    font-family: OptimusPrinceps;
    transition: 0.3s;
  }
  .location:hover{
    text-shadow: 0px 0px 15px #FF6600;
    font-weight: bold;
    transition: 0.3s;
  }
  .home-links a {
  margin-right: 1rem;
  }
  .location_list{
    color:white;
    font-size: 25px;
    display:flex;
    flex-wrap: wrap;
    list-style-type:none;
    align-items:center;
  }
  .location_list li{
    height: 400px;
    width: 400px;
  }
  .location_list li:hover{
    text-shadow: 1px 1px 8px #FF3300;
  }
  .location_img:hover{
    box-shadow: 0 0 10px 3px #FF3300;
  }
  .location_img{
    height: 300px;
    width: 300px;
    object-fit:cover;
    border: 2px solid white;
  }
  .location_img:hover{
    box-shadow: 0 0 10px 3px #FF3300;
  }
</style>
