<!-- COMPONENTE SINGOLO -->
<script>
// SCRIPT
export default {
  data() {
    return {
      content:'-->content goes here <--'

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
    <section class="flex-row container content-padding"><h2>{{ content }}</h2></section>

</template>

<!-- CON SCOPED DICHIARO CSS SOLO AL ATTUALE COMPONENTE/file -->
<style scoped>
/* STILE */
template{
    background-color: black;
}
section{
    height: 7rem;
    color: white;
    font-size: large;
}
h2{
    font-weight: 800;
}
</style>