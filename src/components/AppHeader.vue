<script>
export default {
  data() {
    return { 
      message: ''
    }
  }
}
</script>

<template>
    <header>
      <div class="container">
        <div class="img-header">
          <img src="/img/dc-logo.png" alt="DC Logo">
        </div>
        <nav class="header-links">
          <ul>
            <li>
              <a href="#">
                CHARACTERS
              </a>
            </li>
            <li>
              <a href="#">
                COMICS
              </a>
            </li>
            <li>
              <a href="#">
                MOVIES
              </a>
            </li>
            <li>
              <a href="#">
                TV
              </a>
            </li>
            <li>
              <a href="#">
                GAMES
              </a>
            </li>
            <li>
              <a href="#">
                COLLECTIBLES
              </a>
            </li>
            <li>
              <a href="#">
                VIDEOS
              </a>
            </li>
            <li>
              <a href="#">
                FANS
              </a>
            </li>
            <li>
              <a href="#">
                NEWS
              </a>
            </li>
            <li>
              <a href="#">
                SHOP
              </a>
            </li>
          </ul>
        </nav>
      </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header {
  padding: 20px 0;
}

header ul {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
  
}

header ul li a {
  display: inline-block;
  margin: 5px;
  padding: 10px;
  color: black;
  text-decoration: none;
}

.img-header {
  width: 5%;
}

img {
  max-width: 100%;
}

.header-links {
  width: 80%;
}

</style>
