<template>
  <div>
    <div v-for="page in pages" :key="page.id">
      <Title v-if="page.id === 21" :title="page.title.rendered" />

      <Content
        v-if="page.id === 21"
        class="container"
        :content="page.content.rendered"
      />
    </div>
  </div>
</template>

<script>
import axios from 'axios'
import Title from '@/components/Title'
import Content from '@/components/Content'

export default {
  components: { Title, Content },
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
