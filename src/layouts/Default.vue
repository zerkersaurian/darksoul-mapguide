<template>
  <div class="layout">
    <div class = "nav" @click="goTo('/')">
      <div class="logo"></div>
      <p class="text">Map Guide</p>
    </div>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
  methods: {
    goTo: function(string){
       this.$router.push(string); 
    },
  },
}
</script>

<style>
@font-face{
    font-family: 'OptimusPrinceps';
    src: url(../fonts/OptimusPrincepsSemiBold.ttf);
    font-style:normal;
  }
.logo{
  background-image:url('../picture/index_img/ds3_logo.png');
  background-repeat:no-repeat;
  height: 150px;
  background-position:center;
  transition: 0.3s;
}
.logo:hover{
  background-image:url('../picture/index_img/ds3_logo_hover.png');
  transition: 0.3s;
}
.nav:hover .text{
  text-shadow: 1px 1px 15px #FF6600;
  transition: 0.3s;
}
body {
  font-family: OptimusPrinceps;
  margin:0;
  padding:0;
  line-height: 1.5;
  background-image: url('../picture/Wallpaper.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: bottom right;
}

.layout {
  margin: 0 ;
  text-align:center;
  color:white;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;
  width: 100%;
  background-color: #79DBEF;
}
.text{
  margin: 0;
  font-size: 40px;
}
</style>
