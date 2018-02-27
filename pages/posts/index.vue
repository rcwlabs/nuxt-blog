<template>
  <div class="posts-page">
    <section class="intro">
      <h1 class="intro-text">Get your read on!</h1>
    </section>
    <PostList />
  </div>
</template>

<script>
import PostList from '@/components/Posts/PostList'

export default {
  components: {
      PostList
  }
}
</script>

<style scoped>

.intro {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 300px;
  padding: 1em;
  margin-bottom: 2em;
  background-image: url('~assets/images/coffee-cup-sm.jpg');
  background-size: cover;
}

.intro-text {
  font-size: 3em;
  color: white;
  text-shadow: 2px 2px 2px #333;
}

</style>

