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
      <NuxtLink to="/" target="_blank" prefetch>Home</NuxtLink>
      <NuxtLink to="/about" target="_blank" prefetch>About</NuxtLink>
      <NuxtLink to="/pagina1" target="_blank" prefetch>Pagina1</NuxtLink>
    </div>
      <div>
        <sidebar/>
      </div>
      <div class="main">
        <p>tekst</p>
      </div>
      <div>
        <footer/>
      </div>
  </main>
</template>
<script>
export default {
  transition: 'home'
}
</script>
