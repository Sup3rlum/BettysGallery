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
    width: inherit;
}

.gallery-item-container {
    margin: 5px;
    width: 320px;
}

</style>