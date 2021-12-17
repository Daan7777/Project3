<script>
import bootstrap from '../components/bootstrap.vue'
import footerVue from '../components/footer.vue'
import navbar from '../components/navbar.vue'
export default {
  components: {
    bootstrap,
    footerVue,
    navbar
  },
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