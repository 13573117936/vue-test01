<script>
export default {
  data() {
    return {
      type: 1,
      // ok: true
    }
  },
  methods: {
    add() {
      this.type++
    }
  }
}
</script>

<template>
   <div>
    =============================条件渲染 v-if===============================
  </div>
  <div v-if="type === 1">A</div>
  <div v-else-if="type === 2">B</div>
  <div v-else-if="type === 3">C</div>
  <div v-else>Not A/B/C</div>
  <div>
    <button @click="add">add</button>
  </div>
</template>