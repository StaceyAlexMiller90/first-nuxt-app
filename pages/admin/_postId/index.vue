<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import AdminPostForm from '@/components/Admin/AdminPostForm.vue'

export default Vue.extend({
  layout: 'admin',
  components: {
    AdminPostForm,
  },
  data() {
    return {
      loadedPost: {
        author: 'Stacey',
        title: "Stacey's Great Post!",
        content: 'Great stuff',
        thumbnailLink:
          'https://www.cg.nl/wp-content/uploads/2018/06/tech-header-01.jpg',
      },
    }
  },
})
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>