<script>
export default {
  head: {
    title: 'About pagina',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'about page description'
      }
    ]
  }
}
</script>
<template>
  <main>
    <div>
      <navbar/>
    </div>
    <div>
      <sidebar/>
      <footer/>
    </div>
    <div class="main">
      <p>tekst</p>
    </div>
  </main>
</template>
