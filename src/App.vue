<!-- GRANDE CONTENITORE IN CUI VERRANNO INSERITI UNO AD UNO TUTTTI I COMPONENTI -->
<script>
//IMPORTARE COMPONENTI IMPORT - NOME - FROM - PERCORSO
import AppHeader from './components/AppHeader.vue';
//
import AppContent1 from './components/AppContent1.vue';

import AppContentBlue from './components/AppContentBlue.vue';

import AppFooter  from './components/AppFooter.vue';

// SCRIPT
export default {
  // QUA DICHIARO I COMPONENTI IMPORTATI
  components: {
    // ESEMPIO DI INPORT COMPONENTE
    AppHeader,
    AppContent1,
    AppContentBlue,
    AppFooter,
  },
  data() {
    return {

    }
  },
  methods: {

  },
  mounted() {

  },
}
</script>

<template>
  <!-- TEMPLATE html-->
<AppHeader />
<AppContent1 />
<AppContentBlue />
<AppFooter />

</template>

<style>
/* STILE */
</style>
