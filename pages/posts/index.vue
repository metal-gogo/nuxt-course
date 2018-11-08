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
  data() {
    return {
      posts: [
        {
          author: 'Metal Gogo',
          id: '1',
          title: 'My awesome post',
          content: 'Super amazing content',
          thumbnail: 'http://placekitten.com/600/800',
        },
        {
          author: 'Metal Gogo',
          id: '2',
          title: 'My awesome post 2',
          content: 'Super amazing content',
          thumbnail: 'http://placekitten.com/800/600',
        },
      ],
    };
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
