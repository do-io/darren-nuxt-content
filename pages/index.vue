<template>
  <main>
    <TheHero> DO Dev Blog </TheHero>
    <BlogPostList />
  </main>
</template>

<script setup lang="ts">
import TheHero from "~/components/TheHero.vue";
import BlogPostList from "~/components/BlogPostList.vue";

useHead({
  title: 'Home - DO Dev Blog',
  meta: [
    {
      name: 'description',
      content: 'The DO Dev Blog Head'
    }
  ]
})
</script>
