<script>
import bootstrap from '../components/bootstrap.vue'
import footerVue from '../components/footer.vue'
export default {
  components: {
    bootstrap,
    footerVue
  },
  head: {
    title: 'bergen page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'bergen page description'
      }
    ]
  }
}
</script>
<template>
  <div>
    <div>
      <bootstrap />
      <nav>
        <ul>
          <li>
            <NuxtLink to="/mountain">
              Mountains
            </NuxtLink>
          </li>
          <li>
            <NuxtLink to="/rivers">
              Rivers
            </NuxtLink>
          </li>
        </ul>
      </nav>
      <main>
        <img src="~/assets/logo.svg" />
        <Nuxt />
      </main>
    </div>
    <ul v-for="mountain in mountains" :key="mountain.id">
      <NuxtLink :to="`${mountain.continent.toLowerCase()}/${mountain.slug}`">
        <li>{{ mountain.title }}</li>
      </NuxtLink>
    </ul>
  </div>
  <div>
    <footer />
  </div>
</template>
<script>
export default {
  async asyncData () {
    const mountains = await fetch(
      'https://api.nuxtjs.dev/mountains'
    ).then(function (res) {
      return res.json()
    })

    return { mountains }
  }
}
</script>

<style>
:root {
  --primary-color: #00c58e;
}

body {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto,
    Helvetica Neue, Arial, Noto Sans, sans-serif, Apple Color Emoji,
    Segoe UI Emoji, Segoe UI Symbol, Noto Color Emoji;
  margin: 0;
}

a {
  color: inherit;
  text-decoration: none;
}
nav a:hover {
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

main {
  margin: 0 auto;
  margin-top: 100px;
  padding: 0 1rem;
  max-width: 1280px;
  text-align: center;
}

img {
  margin-bottom: 1rem;
}

ul {
  list-style-type: none;
  padding: 0;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
li {
  margin: 0 0.5rem;
  padding: 0.25rem;
  font-size: 1.2rem;
}

nav {
  padding: 0 1rem;
}
a.nuxt-link-exact-active {
  color: #00c58e;
}
</style>
