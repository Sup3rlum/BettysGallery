<template>
    <div class="imgv-container">
        <div class="imgv-bar"></div>

        <p class="imgv-caption">{{caption}}</p>

        <div class="imgv-img">
            <img class="imgv" :src="path">
            <p class="imgv-text">{{caption}}</p>
        </div>

    </div>
</template>

<script>
export default {
    name: "imageviewer",
    props: ['path', 'caption']
}
</script>

<style>

.imgv-caption {
    margin-top: 15px;
    font-family: 'Montserrat', Geneva, Tahoma, sans-serif;
    font-weight: 300;
    font-size: 17pt;
    display: inline-block;
}

.imgv {

    width: 1000px;
    margin-top: 10px;
    float: left;
}

.imgv-text {
    width: 100px;

}

.imgv-bar {
  margin: 10px;
  width: 1px;
  height: 40px;
  background-color: rgb(255, 238, 0);
  float: left;
}

</style>