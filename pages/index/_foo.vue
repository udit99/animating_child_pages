<template>
  <div>
    <h1>_Foo</h1>
    <NuxtLink to="/foo/bar">Open Grandchild</NuxtLink>
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
  name: "ChildPage",
};
</script>
