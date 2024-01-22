<!-- AuthorInfo.vue -->
<template>
  <div v-if="post.thisBox">
    <!-- Author info modal content goes here -->
    <p class="closeBtn closeBtnP" v-on:click="$emit('close', post.thisBox = false)">&#10006;</p>
    <div id="info_title">{{ post.name }}</div>
    <div id="info_foodie"><span>Foodie Level: </span>{{ post.foodielevel }}</div>
    <div id="info_bio"><span>Bio:<br></span>{{ post.bio }}</div>
    <button class="closeBtn closeBtnB" v-on:click="$emit('close', post.thisBox = false)">Close</button>
    <p id="close_info"></p>
  </div>
</template>

<script>
export default {
  // Component logic goes here
};
</script>

<style scoped>
  /* Component styles go here */
</style>
