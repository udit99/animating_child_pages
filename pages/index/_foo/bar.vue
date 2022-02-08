<template>
  <div>
    <h1>Bar</h1>
    <NuxtLink to="/">Go to Parent</NuxtLink>
    <transition>
      <nuxt-child />
    </transition>
  </div>
</template>

<script>
export default {
  transition: {
    name: "jade",
    mode: "out-in",
  },
  name: "GrandchildPage",
};
</script>
