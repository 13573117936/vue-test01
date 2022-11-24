<script setup>
import Template from './basic/template.vue'
import Reactive from './basic/reactive.vue'
import Computed from './basic/computed.vue'
import Conditional from './basic/conditional.vue'
import List from './basic/list.vue';
import Model from './basic/model.vue';
import Watch from './basic/watch.vue';
import Refs from './basic/refs.vue';
</script>
<template>
  <main>
    <Template />
    <Reactive />
    <Computed />
    <Conditional />
    <List />
    <Model />
    <Watch />
    <Refs />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
