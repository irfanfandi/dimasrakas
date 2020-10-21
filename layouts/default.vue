<template>
  <div>
    <TopNavigation />
    <slide-y-up-transition :duration="400">
      <Nuxt />
    </slide-y-up-transition>
  </div>
</template>

<script>
import { SlideYUpTransition } from 'vue2-transitions'
import TopNavigation from '~/components/Navigation/TopNavigation'

export default {
  components: {
    TopNavigation,
    SlideYUpTransition,
  },
}
</script>

<style></style>
