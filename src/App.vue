<template>
  <Sidebar />

  <router-view />
</template>

<script>
import Sidebar from './components/Sidebar.vue'

export default {
  components: {
    Sidebar
  }
}
</script>


<style>
* {
  margin: 0;
  padding: 0;
	color: #010302;
}

#app {
  font-family: OpenSans, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

a {
  text-decoration: none;
}

/* Carousel styles */

.splide__arrow {
	display: none !important;
}

.splide__pagination {
  bottom: 8px;
}

.splide__pagination__page {
  background: #fff;
  opacity: 1;
}
.splide__pagination__page.is-active {
  background-color: #e63abe;
  transform: scale(1, 1);
}

</style>
