<template>
  <div class="page">
    <Contscts />
    <Gallery />
  </div>
</template>

<script>
import Gallery from '../components/Gallery.vue'
export default {
  components: { Gallery }
}
</script>

<style>
  .page {
    height: 100vh;
    height: 100;
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    padding: 3rem 5rem 0 5rem;
  }
</style>
