<template>
  <div v-html="content" />
</template>

<script>
export default {
  name: 'Content',
  props: {
    content: {
      type: String,
      required: true,
    },
  },
}
</script>

<style>
.paragraph {
  font-size: 1rem;
  color: #00f;
  margin: 1.2rem;
  margin-bottom: 0;
  margin-right: 2.2rem;
  line-height: 1.5rem;
  padding-bottom: 1rem;
}

.subtitle {
  text-align: center;
  font-size: 1.5rem;
  line-height: 1.8rem;
  font-weight: bold;
  color: #060668;
  margin: 1.2rem;
  margin-right: 2.2rem;
}

@media screen and (min-width: 768px) {
  .paragraph {
    font-size: 1.2rem;
    line-height: 1.8rem;
  }

  .subtitle {
    font-size: 1.8rem;
    line-height: 2.2rem;
  }
}

@media screen and (min-width: 1024px) {
  .paragraph {
    font-size: 1rem;
    margin: 1.5rem;
    line-height: 1.5rem;
  }
}
</style>
