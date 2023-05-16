<template>
  <div>
    <button @click="getPosts">Load Posts</button>
  </div>
</template>

<script>
  import axios from "axios"

  export default {
    name: "PostList",
    data() {
      return {
        posts: [],
      }
    },
    methods: {
      getPosts() {
        axios.get('https://jsonplaceholder.typicode.com/posts')
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>