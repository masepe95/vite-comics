<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

import { navbar, dcComics } from '@/assets/data';

export default {
  data() {
    return {
      navbar,
      dcComics
    }
  },
  components: { AppFooter, AppHeader, AppMain }
}

</script>

<template>
  <AppHeader :navbar="navbar" />

  <AppMain />

  <AppFooter />
</template>

<style></style>