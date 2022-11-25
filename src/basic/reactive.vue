<script>
export default {
  data() {
    return {
      count: 0,
      obj: {
        a: {
          num: 1
        },
        b: 2
      }
    }
  },
  methods: {
    add() {
      this.count++
    },
    add2() {
      this.obj.a.num++
    }
  }
}

</script>

<template>
  <div>
    =============================响应式===============================
  </div>
  <div>
    count：{{ count }}
  </div>
  <div>
    obj:{{ obj }}  深层响应式
  </div>
  <div>
    <button @click="add">count + 1</button>
    <button @click="add2">num + 1</button>
  </div>
</template>

<style scoped>
.top {
  margin-top: 20px;
}
</style>