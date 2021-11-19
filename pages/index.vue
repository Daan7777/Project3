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
      <navbar/>
    </div>
      <div>
        <sidebar/>
      </div>
      <div class="main">
        <h1>Header tekst</h1>
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
