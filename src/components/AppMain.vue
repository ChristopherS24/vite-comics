<script>
export default {
  data() {
    return { 
      cards: [
        {
          "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg/revision/latest?cb=20080809201655",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg/revision/latest/scale-to-width-down/1200?cb=20130627211607",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg/revision/latest?cb=20200929145132",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg/revision/latest?cb=20200929124651",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg/revision/latest?cb=20201123054610",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg/revision/latest?cb=20201124094800",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg/revision/latest?cb=20160303223223",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ]
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

      <div class="cards-box" v-for="(card, i) in cards" :key="i">
        <div class="card">
          <img :src="card.thumb" :alt="card.series">
          <p>
            {{ card.series }}
          </p>
        </div>

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

main .cards-box .card {
  width: calc((100% / 6) - 10px);
}

main .cards-box {
  display: flex;
  flex-wrap: wrap;
}

img {
  max-width: 100%;
}

</style>
