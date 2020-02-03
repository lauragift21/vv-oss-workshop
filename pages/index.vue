<template>
  <div class="container">
    <Nav />
    <Gallery />
    <Footer />
  </div>
</template>

<script>
import Nav from '~/components/Nav';
import Gallery from '~/components/Gallery';
import Footer from '~/components/Footer';

export default {
 components: {
   Nav,
   Gallery,
   Footer
 }
}
</script>

<style>
.container {
  border: 39px solid #fcd3d3;
  background: #faeeee;
  min-height: 100vh;
}
</style>
