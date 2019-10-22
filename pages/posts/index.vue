<template>
<div class="container">
  <h1>{{ posts.length }} {{ pluralize('post', posts.length) }}</h1>
  <post v-for="post in posts" :key="post.id" :post="post"></post>
  <a href="#" v-scroll-to="'body'">Back to top</a>
  <!--
    <h1>Posts</h1>
    <p>{{ posts }}</p>
    -->
  </div>
</template>

<script>
import axios from 'axios'
import Post from '@/components/Post'
//import pluralize from 'pluralize'

export default {
  data() {
    return {
      posts: []
    }
  },
  layout: 'posts',
  head: {
    title: 'Posts',
  },
  components: {
    Post
  },
  /*
  methods: {
    pluralize: pluralize
  },
  */
  /*
  // Client side rendering
  mounted() {
    axios.get('https://jsonplaceholder.typicode.com/posts').then((response) => {
      this.posts = response.data
    });
  }
  */
 // Server side rendering (sale)
 /*
  asyncData() {
    return axios.get('https://jsonplaceholder.typicode.com/posts').then((response) => {
      return {
        posts: response.data
      }
    });
  }
  */
 // Sever side rendering (propre)
 async asyncData() {
    let response = await axios.get('https://jsonplaceholder.typicode.com/posts');

    return {
        posts: response.data
      }
  }
}
</script>
