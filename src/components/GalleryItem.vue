<template>
  <div class="gallery-item-container">
    <div class="gallery-item-gradient">
      <div class="gallery-item-bar"/>
    </div>
    <p class="gallery-item-caption">{{ caption }}</p>

    <img :src="path"/>
  </div>
</template>

<script>
export default {
    name: 'galleryitem',
    props: ['path', 'caption']
}
</script>

<style>

img {
    width: inherit;
    box-shadow: 0 4px 4px 0 rgba(14,30,37,.42);
}

.gallery-item-caption {
  font-family: 'Montserrat', sans-serif;
  font-weight: 300;
  padding: 25px;
  margin-left: 10px;
  color: transparent;
  position: absolute;
  transition: 0.4s;

  background-size: cover;
}

.gallery-item-container {
    margin: 5px;
    width: 410px;
    transition: 0.4s;
}
.gallery-item-container:hover > *{
    color: #FFF;
    
}
.gallery-item-container:hover > .gallery-item-gradient{
    opacity: 100%;
    
}
.gallery-item-gradient {
  width: inherit;
  height: 100%;
  background-size: cover;
  opacity: 0;
  position: absolute;
  background-image: linear-gradient(to bottom,rgba(0,0,0,0.6),rgba(0,0,0,0.0));
  transition: 0.4s;
}
.gallery-item-gradient:hover {
    opacity: 100%;
}
.gallery-item-bar {
  margin: 20px;
  width: 1px;
  height: 80px;
  background-color: rgb(255, 238, 0);
}


</style>