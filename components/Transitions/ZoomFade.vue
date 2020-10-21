<template>
  <transition
    enter-active-class="duration-200 ease-out"
    enter-class="opacity-0 scale-95"
    enter-to-class="opacity-100 scale-100"
    leave-active-class="duration-100 ease-in"
    leave-class="opacity-100 scale-100"
    leave-to-class="opacity-0 scale-95"
    v-bind="$attrs"
    v-on="$listeners"
  >
    <slot></slot>
  </transition>
</template>

<script>
export default {
  inheritAttrs: false,
}
</script>

<style></style>
