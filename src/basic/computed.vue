<script>
export default {
  data() {
    return {
      list: [1, 2, 3]
    }
  },
  methods: {
    addLength() {
      this.list.push(1)
    }
  },
  computed: {
    length() {
      return this.list.length
    }
  }
}
</script>

<template>
   <div>
    =============================计算属性 computed===============================
  </div>
  <div>
    length：{{ length }}
  </div>
  <div>
    <button @click="addLength">add</button>
  </div>
</template>