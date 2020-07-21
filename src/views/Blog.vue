<template>
  <div>
      <BlogInfo/>
      <BlogCard/>
  </div>
</template>

<script>
import BlogInfo from '../components/BlogInfo';
import BlogCard from '../components/BlogCard';

export default {
    name: 'blog',
    components: {
        BlogInfo,
        BlogCard,
    }

}
</script>

<style>

</style>