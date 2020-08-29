<template>
  <div class="home-element">
    <a class="home-title" href="#">Betty's Photo Gallery</a>
    <span class="home-scroll-button">Take a look</span>
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
  margin: 200px auto;
  width: 100%;
  text-align: center;
}

.home-title {
  color: #FFF;
  text-decoration: none;
  font-size: 50pt;
  font-family: BlackBerryJam;
}

.home-scroll-button {
  color: #FFF;
  background-color: transparent;
  font-size: 15pt;
  padding: 15px 30px;
  border: 1px solid #EEE;
  border-radius: 20px;
  transition: 0.4s;
}

.home-scroll-button:hover {
  background-color: rgba(153, 151, 151, 0.7);
}

</style>