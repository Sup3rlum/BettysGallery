<template>
  <div class="gallery-item-container">
    <img :src="path"/>
  </div>
</template>

<script>
export default {
    name: 'galleryitem',
    props: ['path', 'imgCaption']
}
</script>

<style>

img {
    border-radius: 5px;
    width: 420px;
}

.gallery-item-container {
    margin: 5px;
}

</style>