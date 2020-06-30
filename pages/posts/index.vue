<template>
  <div class="posts-page">
    <PostList />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import PostList from '@/components/Posts/PostList.vue'

export default Vue.extend({
  components: {
    PostList,
  },
})
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}

.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>