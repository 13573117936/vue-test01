<script>
export default {
  data() {
    return {
      arr: [{ id: 1, name: '张三', age: 20 }, { id: 2, name: '李四', age: 18 }]
    }
  },
}
</script>

<template>
  <div>
    =============================列表渲染 v-for===============================
  </div>
  <div>
    <ul>
      <li v-for="(item, index) in arr" :key="item.id">
        name：{{ item.name }}
        age：{{ item.age }}
        index：{{ index }}
      </li>
    </ul>
  </div>
</template>