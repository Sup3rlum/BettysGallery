<template>
  <div id="app">
    <header>
        <Navbar />
        <HomeButton/>

    </header>
    
    <GalleryWall />

    <footer>
      <span> Copyright Toma Kolev (c) 2020</span>
      <p>toma.kolev@yahoo.com</p>

    </footer>
      <div class="navigation-top-bar">
      </div>
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
}

html {
  scroll-behavior: smooth;
}

body {
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-image: url("../public/assets/water.png");
  background-attachment: fixed;
  background-size: cover;
  background-repeat: no-repeat;
}
header {
  padding: 0px;
  font-family: 'Montserrat', Geneva, Tahoma, serif;
  font-weight: 200;
  font-size: 15pt;
}
footer {
  color: #EEE;
  font-family: 'Montserrat', Geneva, Tahoma, sans-serif;
  font-size: 10pt;
  margin: 0px 0px 100px 100px;
}

</style>