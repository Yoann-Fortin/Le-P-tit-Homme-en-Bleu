<template>
  <header>
    <nav class="navigation">
      <ul>
        <nuxt-link to="/" tag="li">
          <a>
            <span class="icon"><i class="fas fa-home"></i></span>
            <span class="title">Accueil</span>
          </a>
        </nuxt-link>
        <nuxt-link to="/signs" tag="li">
          <a>
            <span class="icon"><i class="fas fa-sign-language"></i></span>
            <span class="title">Les Signes</span>
          </a>
        </nuxt-link>
        <nuxt-link to="/specialists" tag="li">
          <a>
            <span class="icon"><i class="fas fa-user-md"></i></span>
            <span class="title">Les Spécialistes</span>
          </a>
        </nuxt-link>
        <nuxt-link to="/institutions" tag="li">
          <a>
            <span class="icon"><i class="fas fa-hospital-user"></i></span>
            <span class="title">Les Institutions</span>
          </a>
        </nuxt-link>
        <nuxt-link to="/process" tag="li">
          <a>
            <span class="icon"><i class="fas fa-tasks"></i></span>
            <span class="title">Les Démarches</span>
          </a>
        </nuxt-link>
        <nuxt-link to="/associations" tag="li">
          <a>
            <span class="icon"><i class="fas fa-users"></i></span>
            <span class="title">Les Associations</span>
          </a>
        </nuxt-link>
        <nuxt-link to="/adventures" tag="li">
          <a>
            <span class="icon"><i class="fas fa-walking"></i></span>
            <span class="title">Les&#xA0;aventures de Soann</span>
          </a>
        </nuxt-link>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.navigation {
  position: fixed;
  right: 0;
  width: 2rem;
  height: 100%;
  background: #060668;
  transition: 0.5s;
  z-index: 15;
  overflow: hidden;
}

.navigation:hover {
  width: 15rem;
  z-index: 15;
}

.navigation ul {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  color: #d9e0f3;
  display: flex;
  flex-direction: column;
}

.navigation ul li {
  position: relative;
  width: 100%;
  list-style: none;
}

.navigation ul li a {
  position: relative;
  width: 4rem;
  text-decoration: none;
  color: #d9e0f3;
  display: flex;
}

.navigation ul li a .icon {
  position: relative;
  display: block;
  width: 1.5rem;
  height: 1.5rem;
  text-align: center;
  margin: 2rem 2rem 0 0.25rem;
}

.navigation ul li a .icon .fa {
  font-size: 1.5rem;
}

.navigation ul li a .title {
  position: relative;
  display: block;
  height: 1.5rem;
  text-align: start;
  white-space: nowrap;
  margin-top: 2rem;
}

@media screen and (min-width: 768px) {
  .navigation:hover {
    width: 20rem;
  }

  a {
    font-size: 1.2rem;
    line-height: 1.8rem;
  }
}

@media screen and (min-width: 1024px) {
  header {
    height: 5rem;
    width: 100vw;
  }
  .navigation,
  .navigation:hover {
    top: 0;
    left: 0;
    width: 100%;
    height: 5rem;
  }

  .navigation ul {
    flex-direction: row;
    justify-content: space-between;
    margin: 0.5rem;
  }

  .navigation ul li:first-child {
    margin-top: 1.8rem;
    margin-left: 1.5rem;
  }

  .navigation ul li a .icon {
    display: none;
  }

  .navigation ul li a .title {
    white-space: normal;
    font-size: 1.2rem;
    margin: 0.5rem 0.2rem;
  }
}
</style>
