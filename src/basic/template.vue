<script>
export default {
  data() {
    return {
      count: 0,
      rawHtml: `<div>这里是v-html插入的内容</div>`,
      isButtonDisabled: false
    }
  },
  methods: {
    changeState() {
      this.isButtonDisabled = !this.isButtonDisabled
    }
  }
}

</script>

<template>
  <div>
    =============================模板语法===============================
  </div>
  <div>
    <div>~~~~~~~~文本插值~~~~~~~~~</div>
    count：{{ count }}
  </div>
  <div class="top">
    <div>~~~~~~~~v-html插值~~~~~~~~~</div>
    <span v-html="rawHtml"></span>
  </div>
  <div class="top">
    <div>~~~~~~~~v-bind响应式绑定属性~~~~~~~~~</div>
    <button :disabled="isButtonDisabled">{{ isButtonDisabled }}</button>
    <button @click="changeState">changeState</button>
  </div>
</template>

<style scoped>
.top {
  margin-top: 20px;
}
</style>