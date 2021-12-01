<script>
export default {
  head: {
    title: 'Home page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Home page description'
      }
    ]
  }
}
</script>
<template>
  <main>
    <div>
      <bootstrap />
    </div>
    <div class="main">
      <h1>Header tekst</h1>
    </div>
    <div class="main">
      <p>tekst</p>
    </div>
    <div>
      <nav>
        <ul>
          <li>
            <NuxtLink to="/">
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
      <img src="~/assets/logo.svg">
      <Nuxt />
    </div>
    <div class="main">
      <ul v-for="mountain in mountains" :key="mountain.id">
        <NuxtLink :to="`${mountain.continent.toLowerCase()}/${mountain.slug}`">
          <li>{{ mountain.title }}</li>
        </NuxtLink>
      </ul>
    </div>
  </main>
</template>
<script>
export default {
  async asyncData() {
    const mountains = await fetch(
      'https://api.nuxtjs.dev/mountains'
    ).then((res) => res.json())

    return { mountains }
  }
}
</script>
