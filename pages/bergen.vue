<template>
  <div>
      <div>
    <nav>
      <ul>
        <li>
          <NuxtLink to="/mountain">Mountains</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/rivers">Rivers</NuxtLink>
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
