<template>
  <div>
    <h1>editing {{ video.name }}</h1>
    <nuxt-link :to="`/videos/${video.id}`">
      <button>Go Back</button>
    </nuxt-link>
  </div>
</template>

<script>
  export default {
    props: ['video']
  }

</script>

<style lang="scss" scoped>

</style>
