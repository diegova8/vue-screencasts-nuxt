<template>
  <div>
    <h1>We are in video {{ video.name }}</h1>
    <nuxt-link :to="`/videos/${video.id}/edit`">
      <button>Edit</button>
    </nuxt-link>
  </div>
</template>

<script>
  export default {
    props: ['video'],
  }

</script>

<style lang="scss" scoped>

</style>
