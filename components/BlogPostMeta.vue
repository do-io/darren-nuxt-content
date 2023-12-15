<script setup>
const props = defineProps({
  author: {
    type: String,
    required: true
  },
  date: {
    type: String,
    required: true
  },
  color: {
    type: String,
    default: 'info'
  },
  category: {
    type: String,
    default: 'Post'
  },
  tags: {
    type: String, // need to convert to allow array
    default: 'blog'
  }
})

const formattedDate = computed(() => {
  return new Date(props.date).toUTCString()
})
</script>

<template>
  <div class="tags has-addons level-item are-medium">
    <span class="tag is-rounded" :class="`is-${color}`">{{ author }}</span>
    <span class="tag is-rounded">{{ formattedDate }}</span>
  </div>
  <div class="tags has-addons level-item are-medium">
    <span class="tag is-rounded" :class="`is-${color}`">{{ category }}</span>
    <span class="tag is-rounded">{{ tags }}</span>
  </div>
</template>

<style></style>
