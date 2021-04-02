<template>
  <div>
    <Title :title="title" />
    <section v-for="post in posts" :key="post.id">
      <h2>{{ post.title.rendered }}</h2>
      <span v-html="post.content.rendered" />
    </section>
  </div>
</template>

<script>
import axios from 'axios'
import Title from '@/components/Title'

export default {
  components: { Title },
  asyncData() {
    return axios
      .get('http://localhost:8080/wp-json/wp/v2/posts')
      .then((res) => {
        return {
          posts: res.data,
        }
      })
  },
  data() {
    return {
      title: 'Les aventures de Soann',
    }
  },
}
</script>
