<!-- Post.vue -->
<template>
  <li>
    <!-- Blog post content goes here -->
    <span class="profile">
      <img v-bind:src="post.profilepic" v-on:click="authorinfo(posts, post)">
    </span>
    <span class="author">{{ post.name }}</span> — 
    <span class="date">{{ post.date }}</span>
    <span class="reply">{{ post.reply }}</span>
    <p>{{ post.message }}</p>
  </li>
</template>

<script>
export default {
  // Component logic goes here
};
</script>

<style scoped>
  /* Component styles go here */
</style>
