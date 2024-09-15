<script>
export default {
  data() {
    return { 
      headerLinks: [
        {
          label: 'CHARACTERS',
          url: '#'
        },
        {
          label: 'COMICS',
          url: '#'
        },
        {
          label: 'MOVIES',
          url: '#'
        },
        {
          label: 'TV',
          url: '#'
        },
        {
          label: 'GAMES',
          url: '#'
        },
        {
          label: 'COLLECTIBLES',
          url: '#'
        },
        {
          label: 'VIDEOS',
          url: '#'
        },
        {
          label: 'FANS',
          url: '#'
        },
        {
          label: 'NEWS',
          url: '#'
        },
        {
          label: 'SHOP',
          url: '#'
        }

      ]
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
            <li v-for="(link, i) in headerLinks" :key="i">

              <a :href="link.url">
                {{ link.label }}
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

header ul li a:hover {
  color: skyblue;
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
