<template>
      <div>
            <div>I am the child and I didnt animate correctly. Click below to go the grandchild page. This will animate correctly</div>
            <NuxtLink to="/blah/bar">Child page</NuxtLink>
        <transition name="jade" mode="out-in">
          <nuxt-child></nuxt-child>
        </transition>
      </div>
</template>
<style scoped>
.jade-enter-active {
  transition: all .3s ease;
}
.jade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.jade-enter, .jade-leave-to
/* .slide-jade-leave-active below version 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}
</style>
