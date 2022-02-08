<template>
  <div>
    <h1>Parent</h1>
    <NuxtLink to="/foo">Open Child</NuxtLink>
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
  name: "ParentPage",
};
</script>
