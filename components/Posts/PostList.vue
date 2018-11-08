<template>
  <section class="post-list">
    <PostPreview
      id="1"
      title="Post title 1"
      preview-text="Preview text 1"
      thumbnail="http://placekitten.com/200/300"
    />
    <PostPreview
      id="2"
      title="Post title 2"
      preview-text="Preview text 2"
      thumbnail="http://placekitten.com/400/600"
    />
    <PostPreview
      id="3"
      title="Post title 3"
      preview-text="Preview text 3"
      thumbnail="http://placekitten.com/800/1200"
    />
  </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview';
export default {
  components: {
    PostPreview,
  },
};
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
