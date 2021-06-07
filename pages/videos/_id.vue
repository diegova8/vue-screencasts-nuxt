<template>
  <div>
    <nuxt-child :video="video" />
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
    computed: {
      video() {
        return this.videos.find(v => v.id == this.$route.params.id);
      }
    },
  }

</script>

<style lang="scss" scoped>

</style>
