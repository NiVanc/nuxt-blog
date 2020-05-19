<template>
  <div class="posts-page">
    <PostsList :posts="loadedPosts" />
  </div>
</template>

<script>
import PostsList from "~/components/posts/PostsList";

export default {
  components: {
    PostsList
  },
  asyncData(context, callback) {
    setTimeout(() => {
      callback(null, {
        loadedPosts: [
          {
            id: "1",
            title: "First Post",
            previewText: "This is our first post",
            thumbnail:
              "https://www.angelpunk.co/wp-content/uploads/MzI4MDQ2Mg.jpeg"
          },
          {
            id: "2",
            title: "Second Post",
            previewText: "This is our second post",
            thumbnail:
              "https://res.cloudinary.com/people-matters/image/upload/q_auto,f_auto/v1578710070/1578710068.jpg"
          }
        ]
      });
    }, 1500);
  }
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>