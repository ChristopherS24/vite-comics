<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

export default {
  data() {
    return { 
      footerLinksOne: [
        {
          label: 'Characters',
          url: '#'
        },
        {
          label: 'Comics',
          url: '#'
        },
        {
          label: 'Movies',
          url: '#'
        },
        {
          label: 'TV',
          url: '#'
        },
        {
          label: 'Games',
          url: '#'
        },
        {
          label: 'Videos',
          url: '#'
        },
        {
          label: 'News',
          url: '#'
        }
      ],
      footerLinksTwo: [
        {
          label: 'Shop DC',
          url: '#'
        },
        {
          label: 'Shop DC Collectibles',
          url: '#'
        }
      ]
    }
  },
  // 2) Dichiarazione del componente
  components: {
    AppHeader,
    AppMain
  }
}
</script>

<template>
    <!-- Utilizzo del componente -->
    <AppHeader />
    <AppMain />

    <footer>
      <div class="container footer-container">
        <div class="row">

          <div class="links">

            <ul>
              <li>
                <h4>
              DC COMICS
                </h4>
              </li>
              <li v-for="(link, i) in footerLinksOne" :key="i">
                <a :href="link.url">
                  {{ link.label }}
                </a>
              </li>

            </ul>


            <ul>
              <li>
                <h4>
                SHOP
                </h4>
              </li>
              <li v-for="(link, i) in footerLinksTwo" :key="i">
                <a :href="link.url">
                  {{ link.label }}
                </a>
              </li>
              </ul>


            <ul>
              <li>
                <h4>
                  DC
                </h4>
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
              <li>
                <a href="#">
                  link
                </a>
              </li>
            </ul>


            <ul>
              <li>
                <h4>
                SITIES
                </h4>
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

          </div>

        </div>
        
      </div>
    </footer>

    <div class="footerbottom">
      <button>
        SIGN-UP NOW!
      </button>
      <div class="icons">
        <img src="/img/footer-facebook.png" alt="fb">
        <img src="/img/footer-twitter.png" alt="twitter">
        <img src="/img/footer-youtube.png" alt="yt">
        <img src="/img/footer-pinterest.png" alt="pinterest">
        <img src="/img/footer-periscope.png" alt="periscope">
      </div>
    </div>

</template>

<style lang="scss">
@use 'assets/scss/main' as *;

//MAIN
.backgblack {
  background-image: url('/img/jumbotron.jpg');
  height: 350px;
  background-size: 100%;
}

.backgblue {
  width: 100%;
  background-color: skyblue;

}


main .container .main-content-two {
  background-color: skyblue;
  color: white;

}

.infos {
  //background-image: url("/img/buy-comics-merchandise.png");
display: flex;
flex-wrap: wrap;
}

.infos p {
  display: flex;
  align-items: center;
}

.links {
  display: flex;
  width: 100%;
}

//FOOTER
footer {
  background-image: url("/img/footer-bg.jpg");
  background-size: 100% auto;
}

footer h4 {
  color: white;
}

footer ul {
  list-style: none;

}

footer ul li a {
  display: inline-block;
  color: black;
  text-decoration: none;
}


.icons {
  display: flex;
  flex-direction: row-reverse;
  padding: 10px;
}

.footer-container {
  background-image: url(/img/dc-logo-bg.png) ;
  background-repeat: no-repeat;
  background-size: 30%;
  background-position-x: right;
}

.footerbottom {
  background-color: rgb(63, 60, 60);
}

</style>
