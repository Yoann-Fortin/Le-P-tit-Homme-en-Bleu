<template>
  <div>
    <div class="container">
      <Sphere />
    </div>
    <div v-for="page in pages" :key="page.id">
      <Content v-if="page.id === 6" :content="page.content.rendered" />
    </div>
  </div>
</template>

<script>
import axios from 'axios'
import Sphere from '@/components/Sphere'
import Content from '@/components/Content'

export default {
  components: { Sphere, Content },
  asyncData() {
    return axios
      .get(
        'http://yoannfw.cluster030.hosting.ovh.net/blog-autism/wp-json/wp/v2/pages'
      )
      .then((res) => {
        return {
          pages: res.data,
        }
      })
  },
}
</script>

<style>
.container {
  min-height: 100vh;
}
</style>
