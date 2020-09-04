<template>
  <div class="gallery">
    <v-overlay :value="overlay" opacity="0.8">

      <ImageViewer :path="currentImage.imgName" :caption="currentImage.imgCaption" />


      <v-btn
        icon
        @click="overlay = false"
      >
        <v-icon>mdi-close</v-icon>
      </v-btn>
    </v-overlay>

    <div id="gallery-section" class="gallery-wall" v-masonry transition-duration="0.3s" item-selector=".item">
      <div v-masonry-tile class="item" v-for="(image, i) in jsonData.images" :key="i">
        <GalleryItem @click.native="showImage(image)" :path="image.imgName" :caption="image.imgCaption"/>
      </div>
    </div>
  </div>
</template>

<script>

import GalleryItem from './GalleryItem';
import ImageViewer from './ImageViewer';
import data from '../../public/media.json';
import Vue from 'vue';
import {VueMasonryPlugin} from 'vue-masonry';

Vue.use(VueMasonryPlugin);

export default {
    name: 'gallerywall',
    components: {
        GalleryItem,
        ImageViewer
    },
    data () {
      return {
        jsonData: data,
        absolute: true,
        overlay: false,
        currentImage: null
      }
    },
    methods: {
      showImage: function(imageIndex)
      {
        this.currentImage = imageIndex
        this.overlay = true
      }
    }
}
</script>

<style>

.gallery
{
  margin-top: 850px;
  margin-bottom: 100px;
  background-color: #EEE;
}

.gallery-wall {

  padding: 150px 0px 400px 0px;
  margin: 0;

  margin-left: 100px;
}

.gallery-header {
  height: 10px;
  background-color: #444;
}



</style>