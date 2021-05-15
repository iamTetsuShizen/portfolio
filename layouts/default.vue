<template>
  <body>
    <Header />
    <Nuxt />
    <Footer />
  </body>
</template>

<script>
import Header from '../components/organisms/header.vue';
import Footer from '../components/organisms/footer.vue';

export default {
  components: {
    Header,
    Footer
  }
}
</script>
