<!-- COMPONENTE SINGOLO -->
<script>
// SCRIPT
export default {
    // DO UN NOME AL COMPONENTE PER RICONOSCERLO IN CASO DI PROBLEMI
    name: 'card',
    //IMPORTO I PROPS
    props: {
    prodotto: {}
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
      <div class="box"><img :src="prodotto.thumb" alt=""><div class="name">{{ prodotto.series }}</div></div>
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
.name{
    padding-top: 1rem;
    font-size: 1rem;
    font-weight: 700;
}

img{
  width: 100%;
  height: 14rem;
  object-fit: cover;
}

.box{
  width: calc(100% / 6);
  padding: 1rem;
  height: 23rem;
}
</style>