<template>
  <div class="post">
    <h2 class="post__title">
      <nuxt-link :to="{ name: 'posts-id', params: { id: post.id } }">{{ post.title }}</nuxt-link>
      </h2>
    <p>{{ post.body }}</p>
  </div>
</template>

<script>
export default {
  props: {
    post: Object
  }
}
</script>

<style>
/*
  .post {
    margin-bottom: 40px;

    &__title {
      font-size: 3em,
    }

  }
  */
</style>
