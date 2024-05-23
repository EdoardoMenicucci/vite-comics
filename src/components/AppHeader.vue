<!-- COMPONENTE SINGOLO -->
<script>
// SCRIPT
export default {
  data() {
    return {
      // link header
      links: [
        {name: 'characters', url:'#'},
        {name: 'comics', url:'#'},
        {name: 'movies', url:'#'},
        {name: 'tv', url:'#'},
        {name: 'games', url:'#'},
        {name: 'collectibles', url:'#'},
        {name: 'videos', url:'#'},
        {name: 'fans', url:'#'},
        {name: 'news', url:'#'},
        {name: 'shop', url:'#'}
      ],
      urlLogo: '../img/dc-logo.png'

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
  <header class="content-padding flex-row">
    <div class="container flex-row">
      <div><img src="../img/dc-logo.png" alt=""></div>
      <div><span v-for="link ,i in links">{{ link.name.toUpperCase() }}</span></div>
    </div>
  </header>

</template>

<!-- CON SCOPED DICHIARO CSS SOLO AL ATTUALE COMPONENTE/file -->
<style scoped>
/* STILE */
header{
  height: 7rem;
  width: 100%;
  color: rgb(0, 0, 0);
  background-color: white;
  font-weight: 700;
}
span{
  padding: 0 0.6rem;
}
.container{
  align-items: center;
}
</style>
