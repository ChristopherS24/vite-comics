<script>
export default {
  data() {
    return { 

          }
  }
}
</script>

<template>

      <main>
      <div class="backgblack">
        <p>
          CURRENT SERIES
        </p>
      </div>

      <div class="backgblue">
        <div class="container">
          <div class="main-content-two">
            <div class="infos">
              <img src="/img/buy-comics-digital-comics.png" alt="DC Merchandise">
              <p>DIGITAL COMICS</p>

              <img src="/img/buy-comics-merchandise.png" alt="">
              <p>DC MERCHANDISE</p>

              <img src="/img/buy-comics-subscriptions.png" alt="">
              <p>SUBSCRIPTIONS</p>
              
              <img src="/img/buy-comics-shop-locator.png" alt="">
              <p>COMIC SHOP LOCATOR</p>
              
            </div>
          </div>
        </div>
      </div>

    </main>

</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
 
.backgblack {
  position: relative;
}

main .backgblack p {
  position: absolute;
  left: 20px;
  bottom: -10px;
  background-color: rgb(6, 168, 226);
  padding: 7px;
  color: white;
}

</style>
