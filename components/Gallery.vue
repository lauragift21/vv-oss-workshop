<template>
  <div class="main">
    <section class="hero">
      <p>
        Femme Tech is a website dedicated to celebrating the amazing women doing great things in tech.
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
        Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <Women />
    </section>
    <section class="gallery">
      <img
        src="https://res.cloudinary.com/lauragift/image/upload/w_400,h_400/v1562153429/gift5_irlhir.jpg"
        alt="Gift Egwuenu"
      />
      <span>Gift Egwuenu</span>
    </section>
  </div>
</template>

<script>
import Women from '~/components/Women'
export default {
  components: {
    Women
  }
}
</script>

<style scoped>
.main {
  padding-top: 50px;
  margin: 50px;
}
.hero {
  display: flex;
  flex-direction: row;
  height: 70vh;
}
p {
  max-width: 50vw;
  font-size: 1.9rem;
  margin-top: 4rem;
}
svg {
  width: 40%;
  height: auto;
}

img {
  border: 15px solid#f8d1cf;
  outline: none;
  border-radius: 10px;
  height: 450px;
}
</style>