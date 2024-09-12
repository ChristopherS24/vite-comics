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
      <div class="backgblack">
        <div class="container">
          <div class="main-content">
            --&gt; Content goes here &lt;--
          </div>
        </div>
      </div>

      <div class="backgblue">
        <div class="container">
          <div class="main-content-two">
            hola
          </div>
        </div>
      </div>

    </main>

    <footer>
      <div class="container">
        <div class="row">
          <div class="col-1-3">
            <h4>
              DC COMICS
            </h4>
            <ul>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
            </ul>

            <h4>
              SHOP
            </h4>
            <ul>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              </ul>

              <h4>
              DC
            </h4>
            <ul>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
            </ul>

            <h4>
              SITIES
            </h4>
            <ul>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
              <li>
                <a href="#">
                  link
                </a>
              </li>
            </ul>

          </div>
        </div>
      </div>
    </footer>

</template>

<style lang="scss">
@use 'assets/scss/main' as *;

//MAIN
.backgblack {
  width: 100%;
  background-color: black;
}

.backgblue {
  width: 100%;
  background-color: skyblue;

}

main .container .main-content {
  text-align: left;
  font-size: 2rem;
  color: white;
  width: 100%;
}

main .container .main-content-two {
  background-color: skyblue;
  color: white;

}

//FOOTER
footer {
  background-image: url("/img/footer-bg.jpg")
}
</style>
