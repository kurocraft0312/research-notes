<template lang="pug">
  section.container
    ul
      li(v-for="post in posts" :key="post.id") {{post.id}}:{{post.title}}、{{post.content}}、
        img(:src="'http://localhost:1337/${post.cover.url}'")
</template>
