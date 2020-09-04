<template>
  <div class="home-element">
    <a class="home-title" href="#">Betty's Photo Gallery</a>
    <a class="home-scroll-button" href="#gallery-section">Take a look</a>
  </div>
</template>

<script>

export default {
    name: 'homebutton'
  
}
</script>

<style>

.home-element {
  float: left;
  margin: 260px auto;
  width: 100%;
  text-align: center;
}

.home-title {
  color: #FFF;
  text-decoration: none;
  font-size: 60pt;
  font-family: BlackBerryJam;
  padding: 10px;
/*
  background-image: -webkit-gradient(linear, left top, right bottom, color-stop(0, #faf), color-stop(1, #aff));
  background-image: gradient(linear, left top, right bottom, color-stop(0.15, #f2f), color-stop(0.45, #2ff));
  color:transparent;
  -webkit-background-clip: text;
  background-clip: text;
  */
}

.home-scroll-button {
  color: #FFF;
  background-color: transparent;
  font-size: 15pt;
  padding: 15px;
  text-decoration: none;

  transition: 0.4s;
  display: block;

  border: 1px solid #FFF;
  border-radius: 20px;  
  margin: auto;
  margin-top: 30px;
  width: 150px;
  
}

.home-scroll-button:hover {
  color: black;
  background-color: rgb(255,255,255);
}

</style>