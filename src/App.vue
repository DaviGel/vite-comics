<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  },
};
</script>

<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponent />
</template>

<style>
body {
  font-family: 'Asap Condensed', sans-serif;
  font-family: 'Lato', sans-serif;
}

img {
  display: block;
  max-width: 100%;
}

.t-upper {
  text-transform: uppercase;
}

.container {
  max-width: 1270px;
  margin: 0 auto;
}
</style>
