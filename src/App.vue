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
    <!-- Utilizzo del componente -->
    <AppHeader />


    
    <main>
      <div class="container">
        <div class="main-content">
          --&gt; Content goes here &lt;--
        </div>
      </div>

      <div class="container">
        <div class="main-content-two">
          hola

        </div>

      </div>
    </main>

    <footer>
      <div class="container">
        <div class="row">
          <div class="col-1-3">
            <img src="/img/footer-bg.jpg" alt="footerback">
          </div>
          <div class="col-1-3">

          </div>

        </div>
        footer
      </div>
    </footer>

</template>

<style lang="scss">
@use 'assets/scss/main' as *;


main .main-content {
  text-align: left;
  font-size: 2rem;
  color: white;
  background: black
}

main .main-content-two {
  background-color: skyblue;
  color: white;
}
</style>
