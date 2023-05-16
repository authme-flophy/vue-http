<template>
  <div>
    <!-- <button @click="getPosts">Load Posts</button> -->
    <h3 v-if="errMsg">{{ errMsg }}</h3>
    <div v-for="post in posts" :key="post.id">
      <h1>{{ post.title }}</h1>
      <p>{{ post.body }}</p>
    </div>
  </div>
</template>

<script>
  import axios from "axios"

  export default {
    name: "PostList",
    created() {
      this.getPosts()
    },
    data() {
      return {
        posts: [],
        errMsg: ""
      }
    },
    methods: {
      getPosts() {
        axios
          .get('https://jsonplaceholder.typicode.com/posts')
          .then((response) => {
            console.log(response.data)
            this.posts = response.data
          })
          .catch(err => {
            console.log(err)
            this.errMsg = "Error retrieving data"
          })
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>