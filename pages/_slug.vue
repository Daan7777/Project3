<template>
  <div>
    <h1>{{ slug }}</h1>
    <p>Path: {{ $route.path }}</p>
  </div>
</template>
<script>
export default {
  async asyncData ({ params }) {
    const slug = await fetch(
      params.slug
    )
    return { slug }
  }
}
</script>
