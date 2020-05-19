<template>
  <section class="posts-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://res.cloudinary.com/people-matters/image/upload/q_auto,f_auto/v1578710070/1578710068.jpg"
      title="Hello there!"
      previewText="Don't hesitate. Click to read more."
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://www.angelpunk.co/wp-content/uploads/MzI4MDQ2Mg.jpeg"
      title="More exciting news!"
      previewText="I know you're tempted. Just click to read more."
    />
    <PostPreview
      id="3"
      :is-admin="isAdmin"
      thumbnail="https://lh3.googleusercontent.com/proxy/_nhMHrzRvqRsZ_ku43iueQ9fxeT18gSIYVQQSsyO7CzYsDLB41SPdvZ7eEGAtO5E9Pq9HyJjJnbf0LscYxXZxQAYJv4Bib_74tIpCz7Ub1M9LfpW4HmE7pGwIKu4SPsDwqzTAW4I5YR4LElsPwpxs5Ijow"
      title="Clickbait title"
      previewText="You must click this one for sure."
    />
  </section>
</template>

<script>
import PostPreview from "~/components/posts/PostPreview";

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
};
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