<template>
  <div class="gallery">
    <div class="gallery-header">
    </div>

    <div class="gallery-wall" v-masonry transition-duration="0.3s" item-selector=".item">
      <div v-masonry-tile class="item" v-for="(image, i) in images" :key="i">
        <GalleryItem :path="image.imgName"/>
      </div>
    </div>
  </div>
</template>

<script>

import GalleryItem from './GalleryItem';
import Vue from 'vue';
import {VueMasonryPlugin} from 'vue-masonry';

Vue.use(VueMasonryPlugin);

export default {
    name: 'gallerywall',
    components: {
        GalleryItem
    },
    data () {
      return {
        images : [
          {
            imgName: '/assets/media/img1.jpg',
            imgCaption: 'A beautiful mountain side'
          },
          {
            imgName: '/assets/media/img2.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img3.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img4.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img5.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img6.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img7.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
                    {
            imgName: '/assets/media/img8.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img9.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img10.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img11.png',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img12.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img13.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img14.jpg',
            imgCaption: 'Landscape of epic proportions'
          },
          {
            imgName: '/assets/media/img15.jpeg',
            imgCaption: 'Landscape of epic proportions'
          }
        ]
      }
    }
}
</script>

<style>

.gallery-wall {

  padding: 140px 0px 400px 0px;
  margin: 250px 0;
  background-color: #EEE;

}

</style>