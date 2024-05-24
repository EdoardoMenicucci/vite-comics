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
      <div><img :src="urlLogo" alt=""></div>
      <div><span class="links" v-for="link ,i in links">{{ link.name.toUpperCase() }} <span class="underline"></span> </span></div>
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
.links{
  padding: 0 0.6rem;
  position: relative;
}

.links:hover{
  color: rgb(40, 40, 255);
}


.underline{
  display: none;
  position: absolute;
  height: 5px;
  width: 100%;
  bottom: -3rem;
  left: -0rem;
}

.links:hover .underline{
  display: block;
  border-bottom: 3px solid blue;
  color: rgb(49, 49, 255);
}

.container{
  align-items: center;
}
</style>
