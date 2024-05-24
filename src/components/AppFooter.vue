<!-- COMPONENTE SINGOLO -->
<script>
// SCRIPT
export default {
  data() {
    return {
      dcComics:[
      'Characters','Comics','Movies','TV','Games','Videos','News'
      ],
      shop: [
        'shop DC', 'Shop DC Collectibles'
      ],
      dc:[
        'Terms Of Use','Privact policy','Ad Choise','Advertising','Jobs','Subscription','Talent Workshops','CPSC Certificate','Ratings','Shop Help','Contact Us'
      ],
      sites: [
        'DC','MAD Magazines','DC Kids','DC Universe','DC Power Visa'
      ],
      urlImg: '/img/dc-logo-bg.png'
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
  <footer class="pt-5">
    <div class="container d-flex">
      <div class="left-column flex-columns">
         <h2>DC COMICS</h2>
          <a href="#" v-for="elemento , i in dcComics">{{ elemento }}</a>
          <h2 class="pt-5">SHOP</h2>
          <a href="#" v-for="elemento , i in shop">{{ elemento }}</a>
      </div>
      <div class="ps-3 left-column flex-columns">
         <h2>DC</h2>
          <a href="#" v-for="elemento , i in dc">{{ elemento }}</a>
      </div>
      <div class="ps-3 left-column flex-columns">
         <h2>SITES</h2>
          <a href="#" v-for="elemento , i in sites">{{ elemento }}</a>
      </div>
      <div class="ps-5">
         <img :src="urlImg" alt="">
      </div>
    </div>
  
  </footer>


</template>

<!-- CON SCOPED DICHIARO CSS SOLO AL ATTUALE COMPONENTE/file -->
<style scoped>
/* STILE */
.left{
  width: 20%;
}
a{
  text-decoration: none;
  color: white;
  font-size: 1.2rem;
  opacity: 0.5;
}
h2 {
  font-weight: 700;
}
footer {
  height: 30rem;
  width: 100%;
  background-image: url(/public/img/footer-bg.jpg);
  position: relative;
}

img{
  height: 100%;
  position: absolute;
  top: 0rem;
  right: 25rem;
  z-index: 1;
}
</style>