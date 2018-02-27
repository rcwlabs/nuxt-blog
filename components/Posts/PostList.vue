<template>
  <section class="post-list">
      <PostPreview 
        id="1" 
        title="This is a great title" 
        previewText="This is the awesome preview text.  And here is some more. This is the awesome preview text.  And here is some more."
        thumbnail="https://cdn.arstechnica.net/wp-content/uploads/2012/08/Commodore64-640x404.jpg"
      />
      <PostPreview 
        id="2" 
        title="This title is not good" 
        previewText="This is the awesome preview text.  And here is some more. This is the awesome preview text.  And here is some more."
        thumbnail="https://cdn.arstechnica.net/wp-content/uploads/2012/08/Commodore64-640x404.jpg"
      />
      <PostPreview 
        id="3" 
        title="This title is like a hotdog" 
        previewText="This is the awesome preview text.  And here is some more. This is the awesome preview text.  And here is some more."
        thumbnail="https://cdn.arstechnica.net/wp-content/uploads/2012/08/Commodore64-640x404.jpg"
      /> 
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
      PostPreview
  }
}
</script>

<style scoped>

.post-list {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

</style>

