<template>
  <nav>
    <a href="#" class="fa fa-instagram"></a>
    <div class="menu-item"><a href="#">About</a></div>
    <Dropdown title="Services" :items="services" />
    <div class="menu-item"><a href="#">Contact</a></div>
  </nav>
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
nav {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  margin: 50px 50px;
}
nav .menu-item {
  color: #FFF;
  padding: 10px 20px;
  position: relative;
  text-align: center;
  border-bottom: 3px solid transparent;
  display: inline-flex;
  transition: 0.4s;
}
nav .menu-item.active,
nav .menu-item:hover {
  background-color: tranparent;
  border-bottom-color: #FF5858;
}
nav .menu-item a {
  color: inherit;
  text-decoration: none;
}
.fa
{
  padding: 20px;
}
.fa-instagram
{
  color: #FFF;

}
</style>