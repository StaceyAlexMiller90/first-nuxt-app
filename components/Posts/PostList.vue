<template>
  <section class="posts-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://www.cg.nl/wp-content/uploads/2018/06/tech-header-01.jpg"
      title="Hello this is a post"
      previewText="This is a preview"
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://www.cg.nl/wp-content/uploads/2018/06/tech-header-01.jpg"
      title="Hello this is a 2nd post"
      previewText="This is a 2nd preview"
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://www.cg.nl/wp-content/uploads/2018/06/tech-header-01.jpg"
      title="Hello this is a 3rd post"
      previewText="This is a 3rd preview"
    />
  </section>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: {
    isAdmin: {
      type: Boolean,
      default: false,
    },
  },
})
</script>

<style scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
</style>