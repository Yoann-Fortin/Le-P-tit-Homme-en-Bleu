<template>
  <div>
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
export default {
  name: 'Title',
  props: {
    title: {
      type: String,
      required: true,
    },
  },
}
</script>

<style scoped>
h1 {
  font-family: 'Playfair Display', serif;
  font-size: 2.5rem;
  line-height: 3rem;
  text-align: center;
  font-weight: bold;
  color: #060668;
  text-shadow: black 1px 1px 1px;
  margin: 1.2rem;
  margin-right: 2.2rem;
  margin-top: 0;
  padding-top: 2rem;
}

@media screen and (min-width: 768px) {
  h1 {
    font-size: 4rem;
    line-height: 6rem;
  }
}

@media screen and (min-width: 1024px) {
  h1 {
    font-size: 6rem;
    line-height: 9rem;
  }
}
</style>
