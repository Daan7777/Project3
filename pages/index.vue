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
    <div class="navbar nuxt-link-active">
      <NuxtLink to="/" target="_blank" prefetch>Home page</NuxtLink>
      <NuxtLink to="/about" target="_blank" prefetch>about</NuxtLink>
      <NuxtLink to="/pagina1" target="_blank" prefetch>Test pagina</NuxtLink>
    </div>
      <div>
        <sidebar />
      </div>
      <div class="main">
        <p>tekst</p>
      </div>
  </main>
</template>
<script>
export default {
  transition: 'home'
}
</script>
