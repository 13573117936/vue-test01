<script>
export default {
  data() {
    return {
      count: 0
    }
  },
  methods: {
    add() {
      this.count++
    }
  },
  watch: {
    count: {
      handler() {
        console.log('count change')
      },
      immediate: true,
      deep: true
    }
  }
}
</script>

<template>
  <div>
    =============================数据监听 watch===============================
  </div>
  <div>count：{{ count }}</div>
  <div>
    <button @click="add">count + 1</button>
  </div>
</template>