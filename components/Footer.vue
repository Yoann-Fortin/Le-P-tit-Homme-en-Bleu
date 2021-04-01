<template>
  <footer>
    <nav>
      <ul>
        <nuxt-link to="/about" tag="li">
          <a>Qui sommes-nous</a>
        </nuxt-link>
        <nuxt-link to="/contact" tag="li">
          <a>Nous contacter</a>
        </nuxt-link>
        <nuxt-link to="/links" tag="li">
          <a>Les liens utiles</a>
        </nuxt-link>
      </ul>
    </nav>
    <p>Le P'tit Homme en Bleu - 2021</p>
  </footer>
</template>

<style scoped>
footer {
  height: 5rem;
  background-color: #060668;
  color: #d9e0f3;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}

ul {
  display: flex;
  justify-content: space-around;
}
a {
  text-decoration: none;
  font-size: 0.8rem;
}

a:visited {
  text-decoration: none;
  color: #d9e0f3;
}

p {
  text-align: center;
}

@media screen and (min-width: 768px) {
  a {
    font-size: 1rem;
  }
}
</style>
