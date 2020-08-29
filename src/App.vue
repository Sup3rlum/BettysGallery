<template>
  <div id="app">
    <header>
        <HomeButton/>
        <Navbar />
        <GalleryWall />
    </header>
    
  </div>
</template>

<script>
import Navbar from './components/Navbar';
import HomeButton from './components/HomeButton';
import GalleryWall from './components/GalleryWall';

export default {
  name: 'app',
  components: {
    Navbar,
    HomeButton,
    GalleryWall
  }
}
</script>

<style>

@font-face { font-family: BlackBerryJam; src: url('../public/assets/BlackberryJamPersonalUse-rXOB.ttf'); } 

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-image: url("../public/assets/media/Untitled.png");
  background-attachment: fixed;
  background-size: cover;
  background-repeat: no-repeat;
}
header {
  padding: 0px;
  font-family: 'Montserrat', Geneva, Tahoma, sans-serif;
  font-size: 15pt;
}

</style>