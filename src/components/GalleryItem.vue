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
    box-shadow: 0 4px 4px 0 rgba(14,30,37,.42);
}

.gallery-item-container {
    margin: 5px;
    width: 320px;

}

</style>