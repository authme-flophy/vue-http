<template>
  <TemplateRef/>

  <!-- <PostList/>
  <CreatePost/> -->
</template>

<script>
import CreatePost from './components/CreatePost.vue';
import HelloWorld from './components/HelloWorld.vue'
import PostList from './components/PostList.vue';
import TemplateRef from './components/TemplateRef.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    PostList,
    CreatePost,
    TemplateRef,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
