<template>
  <div class="container">
    <Nav />
    <Gallery />
  </div>
</template>

<script>
import Nav from '~/components/Nav';
import Gallery from '~/components/Gallery';

export default {
 components: {
   Nav,
   Gallery
 }
}
</script>

<style>
.container {
  border: 9px solid pink;
  min-height: 100vh;
}
</style>
