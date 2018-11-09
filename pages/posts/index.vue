<template>
  <div class="posts-page">
    <PostList :posts="posts" />
  </div>
</template>

<script>
import PostList from '@/components/Posts/PostList';

export default {
  components: {
    PostList,
  },
  asyncData(context, callback) {
    setTimeout(() => {
      callback(null, {
        posts: [
          {
            author: 'Metal Gogo',
            id: '1',
            title: 'My awesome post',
            previewText: 'Super amazing content',
            thumbnail: 'http://placekitten.com/600/800',
          },
          {
            author: 'Metal Gogo',
            id: '2',
            title: 'My awesome post 2',
            previewText: 'Super amazing content',
            thumbnail: 'http://placekitten.com/800/600',
          },
        ],
      });
    }, 1000);
  },
};
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
