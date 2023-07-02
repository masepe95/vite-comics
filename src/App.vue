<script>
import _dcComics from './assets/data/_dc-comics';
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

import { navbar, comics } from '@/assets/data';

export default {
  data() {
    return {
      navbar,
      comics
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