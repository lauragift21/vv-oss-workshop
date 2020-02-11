<template>
  <div class="main">
    <section class="hero">
      <p>
        Femme Tech is a project dedicated to celebrate the amazing women we have in the tech industry.
        Women continue to strive wherever we find ourselves and we don't just
        <b>meet</b> expectations we
        <b>exceed</b> them.
        Let's all keep winning 🎉
      </p>
      <Women />
    </section>
    <section class="gallery">
      <div :key="key" v-for="(profile, key) in profiles">
        <a :href="profile.twitter">
          <img :src="profile.image" alt="Gift Egwuenu" />
          <br />
          <span> <b>{{profile.name}}</b></span>
          <br />
          <span>  {{profile.role}} 👩‍💻</span>
          <br />
          <span> {{profile.Zodiac}} ⭐</span>
        </a>
      </div>
    </section>
  </div>
</template>

<script>
import Women from '~/components/Women'
import { mapState } from 'vuex'

export default {
  components: {
    Women
  },
  computed: {
    ...mapState(['profiles'])
  }
}
</script>

<style scoped>
.main {
  padding-top: 50px;
  font-family: 'Martel Sans', sans-serif;
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
a {
  text-decoration: none;
  color: #000;
  cursor: pointer;
}

img {
  border: 15px solid#f8d1cf;
  outline: none;
  border-radius: 10px;
  height: 300px;
}

.gallery {
  display: grid;
  grid-template-rows: auto;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
  text-align: center;
}
</style>