<template>
  <p :id="id">{{ content }}</p>
</template>

<script>
export default {
  name: 'Paragraph',
  props: {
    id: {
      type: String,
      required: true,
    },
    content: {
      type: String,
      required: true,
    },
  },
}
</script>

<style scoped>
p {
  font-size: 1rem;
  color: #060668;
  margin: 1.2rem;
  margin-bottom: 0;
  margin-right: 2.2rem;
  line-height: 1.5rem;
  padding-bottom: 1rem;
}

@media screen and (min-width: 768px) {
  p {
    font-size: 1.2rem;
    margin: 1.2rem;
    line-height: 1.8rem;
  }
}

@media screen and (min-width: 1024px) {
  p {
    font-size: 1.5rem;
    margin: 1.5rem;
    line-height: 2rem;
  }
}
</style>
