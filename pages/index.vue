<template>
          <div>
            <div>Click below to go the child page. This will not animate, it'll just pause for 500ms and render the child page</div>
            <NuxtLink to="/blah">Child page</NuxtLink>
            <transition name="jade" mode="out-in">
              <nuxt-child></nuxt-child>
            </transition>
          </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
<style scoped>
.jade-enter-active {
  transition: all 500ms ease;
}
.jade-leave-active {
  transition: all 500ms cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.jade-enter, .jade-leave-to
/* .slide-jade-leave-active below version 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}
</style>
