<template>
  <div class="navigation-header">
    <div class="navigation-top-bar">
    </div>

    <nav>

      <div class="menu-item"><a href="https://www.youtube.com/watch?v=oHg5SJYRHA0" class="fa fa-instagram"></a></div>
      <div class="menu-item"><a href="#">About Me</a></div>
      <div class="menu-item"><a href="#">Contact Me</a></div>
      <Dropdown title="Services" :items="services" />
    </nav>
  </div>
</template>

<script>
import Dropdown from './Dropdown';

export default {
  name: 'navbar',
  components: {
    Dropdown
  },
  data () {
    return {
      services: [
        {
          title: 'Web',
          link: '#'
        },
        {
          title: 'Design',
          link:'#'
        },
        {
          title: 'Videos',
          link: '#'
        }
      ]
    }
  }
}
</script>

<style>


.navigation-top-bar {
  height: 10px;
  background-color: transparent;
}





.navigation-header {
  margin-top: 20px;
  height: 80px;
  background-color: rgba(0,0,0,0.0);
}

nav {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  margin: auto;

}
nav .menu-item {
  color: #FFF;
  padding: 20px 20px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: inline-flex;
  transition: 0.4s;
}


nav .menu-header a
{
  text-decoration: none;
  color: #FFF;
  margin: 35px 20px;
}

nav .menu-item.active,
nav .menu-item:hover {
  background-color: tranparent;
  border-bottom-color: #FFF;
}
nav .menu-item a {
  color: inherit;
  text-decoration: none;
}


.fa
{
  padding: px;
}
.fa-instagram
{
  color: #FFF;
}
</style>