<template>
  <div>
    <nuxt-child />
    <h1>Videos</h1>
    <div v-for="video in videos" :key="video.id">
        <nuxt-link :to="`/videos/${video.id}`">{{ video.name }}</nuxt-link>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        videos: [{
            id: '1',
            name: 'Intro to Nuxt'
          },
          {
            id: '2',
            name: 'Intro to VueJs'
          },
          {
            id: '3',
            name: 'Advanced Frameworks'
          }
        ]
      }
    },
  }

</script>

<style lang="scss" scoped>

</style>
