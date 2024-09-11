<script>
import AppHeader from './components/AppHeader.vue';

export default {
  data() {
    return
    
  },
  // Dichiarazione del componente
  components: {
    AppHeader
  }
}
</script>

<template>
  <div>
    <!-- Utilizzo del componente -->
    <AppHeader />

    <header>
      header
    </header>
    
    <main>
      main
    </main>

    <footer>
      footer
    </footer>

  </div>
</template>

<style lang="scss">
@use 'assets/scss/main' as *;
</style>
