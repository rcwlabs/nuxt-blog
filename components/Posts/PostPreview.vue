<template>
    <nuxt-link :to="'/posts/' + id">
        <article class="post-preview">
            <div 
                class="post-thumb"
                :style="{backgroundImage: 'url(' + thumbnail + ')'}">
            </div>
            <div class="post-content">
                <h1>{{title}}</h1>
                <p>{{previewText}}</p>
            </div>
        </article>
    </nuxt-link>
</template>

<script>
export default {
  name: 'PostPreview',
  props: {
      id: {
          type: String,
          required: true
      },
      title: {
          type: String,
          required: true
      },
      previewText: {
          type: String,
          required: true
      },
      thumbnail: {
          type: String,
          required: true
      }
  }
}
</script>


<style>

.post-preview {
  max-width: 33%;
  min-width: 320px;
  text-align: center;
  box-shadow: 1px 2px 2px #777;
  padding: 1em;
}

.post-thumb {
    width: 100%;
    height: 150px;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

</style>
