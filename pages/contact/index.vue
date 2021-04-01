<template>
  <Title :title="title" />
</template>

<script>
import Title from '@/components/Title'

export default {
  components: { Title },
  data() {
    return {
      title: 'Nous contacter',
    }
  },
}
</script>
