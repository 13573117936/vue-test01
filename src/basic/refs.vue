<script>
export default {
  data() {
    return {
      list: [1, 2, 3]
    }
  },
  mounted() {
    console.log(this.$refs.items)
  }
}
</script>

<template>
  <div>
    =============================模板引用 Refs===============================
  </div>
  <ul>
    <li v-for="item in list" ref="items">
      {{ item }}
    </li>
  </ul>
</template>