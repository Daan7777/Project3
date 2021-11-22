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
      <navbar />
    </div>
    <div>
      <sidebar />
    </div>
    <div class="main">
      <h1>Header tekst</h1>
    </div>
    <div class="main">
      <p>tekst</p>
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
