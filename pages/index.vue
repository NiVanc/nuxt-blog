<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news.</h1>
    </section>
    <div class="featured-posts">
      <PostPreview
        id="1"
        thumbnail="https://res.cloudinary.com/people-matters/image/upload/q_auto,f_auto/v1578710070/1578710068.jpg"
        title="Hello there!"
        previewText="Don't hesitate. Click to read more."
      />
      <PostPreview
        id="2"
        thumbnail="https://www.angelpunk.co/wp-content/uploads/MzI4MDQ2Mg.jpeg"
        title="More exciting news!"
        previewText="I know you're tempted. Just click to read more."
      />
      <PostPreview
        id="3"
        thumbnail="https://lh3.googleusercontent.com/proxy/_nhMHrzRvqRsZ_ku43iueQ9fxeT18gSIYVQQSsyO7CzYsDLB41SPdvZ7eEGAtO5E9Pq9HyJjJnbf0LscYxXZxQAYJv4Bib_74tIpCz7Ub1M9LfpW4HmE7pGwIKu4SPsDwqzTAW4I5YR4LElsPwpxs5Ijow"
        title="Clickbait title"
        previewText="You must click this one for sure."
      />
    </div>
  </div>
</template>

<script>
import PostPreview from "~/components/posts/PostPreview";

export default {
  components: {
    PostPreview
  }
};
</script>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
