<template>
  <div admin-post-page>
    <section class="update-form">
      <AdminPostForm :post="LoadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "~/components/Admin/AdminPostForm";

export default {
  components: {
    AdminPostForm
  },
  data() {
    return {
      LoadedPost: {
        author: "Nico",
        title: "My awesome post",
        content: "Super amazing content here.",
        thumbnailLink:
          "https://www.angelpunk.co/wp-content/uploads/MzI4MDQ2Mg.jpeg"
      }
    };
  }
};
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