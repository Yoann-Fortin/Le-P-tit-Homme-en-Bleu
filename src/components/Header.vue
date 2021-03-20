<template>
  <header>
    <nav>
      <ul>
        <li><img src="../../src/assets/Logo.svg" alt=""></li>
        <li>Les Signes</li>
        <li>Les Spécialistes</li>
        <li>Les Institutions</li>
        <li>Les Démarches</li>
        <li>Les Associations</li>
        <li>L'aventure de Soann</li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped>
header {
  height: 5rem;
  padding: 1rem;
}

ul {
  display: flex;
  justify-content: space-around;
}

li {
  color: blue;
  font-size: 1.5rem;
  font-weight: bold;
  margin: auto 1rem;
}

img {
  max-height: 4rem;
}
</style>