<!-- COMPONENTE SINGOLO -->
<script>
// SCRIPT
export default {
  data() {
    return {
      arrayObjects:[
        {name: 'digital comics', url: '/img/buy-comics-digital-comics.png'},
        {name: 'dc merchandise', url: '/img/buy-comics-merchandise.png'},
        {name: 'subscription', url: '/img/buy-comics-subscriptions.png'},
        {name: 'comic shop locator', url: '/img/buy-comics-shop-locator.png'},
        {name: 'dc powered visa', url: '/img/buy-dc-power-visa.svg'},
      ],
    

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
  <div class="bg-blue z-positive">
    <section class="flex-row container">
        <span v-for="elemento , i in arrayObjects"><img :src="elemento.url" alt="">{{ elemento.name }}</span>
    </section>
</div>

</template>

<!-- CON SCOPED DICHIARO CSS SOLO AL ATTUALE COMPONENTE/file -->
<style scoped>
/* STILE */
.bg-blue{
    background-color: rgb(59, 65, 255);
}
section{
    height: 9rem;
    color: white;
    font-size: 1.2rem;
}
img{
    height: 4rem;
    max-width: 6rem;
    padding: 0 0.5rem;
}
</style>