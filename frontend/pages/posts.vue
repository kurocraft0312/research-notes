<template lang="pug">
  section.container
    ul
      li(v-for="post in posts" :key="post.id") {{post.id}}:{{post.title}}、{{post.content}}、
        img(:src="'http://localhost:1337/${post.eyecatch.url}'")
</template>
<script>
import axios from 'axios'

export default {

  async asyncData({app}){
    let res = await axios.get('http://localhost:1337/posts')
    return {posts : res.data}
  }
}
</script>
