<template>
  <div>
    <form>
      <div>
        <label for="userId">Post User Id</label>
        <input type="text" name="userId" id="userId" v-model="formData.userId">
      </div>
      <div>
        <label for="title">Post title</label>
        <input type="text" name="title" id="title" v-model="formData.title">
      </div>
      <div>
        <label for="body">Post Body</label>
        <input type="text" name="body" id="body" v-model="formData.body">
      </div>
      <button>Create Post</button>
    </form>
  </div>
</template>

<script>
  export default {
    name: "CreatePost",
    data() {
      return {
        formData: {
          userId: "",
          title: "",
          body: ""
        }
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>