<script>
export default {
  data() {
    return {
      name: '',
      age: 1,
      info: '',
      checkNames: [],
      pick: '',
      select: ''
    }
  },
}
</script>

<template>
  <div>
    =============================输入绑定 v-model===============================
  </div>
  <div>~~~~~~~~输入框绑定~~~~~~~~~</div>
  <div>
    <label for="a">name：</label>
    <input name="a" v-model="name">
    age：<input v-model="age">
    text：<textarea v-model="info"></textarea>
  </div>
  <div>
    name：{{ name }} age：{{ age }}
    <p style="white-space: pre-line;">text：{{ info }}</p>
  </div>
  <div>~~~~~~~~单选框绑定~~~~~~~~~</div>
  <div>
    <input type="radio" value="one" name="one" v-model="pick">
    <label for="one" style="margin-right:10px">one</label>
    <input type="radio" value="two" name="two" v-model="pick">
    <label for="two">two</label>
    <div>pick：{{ pick }}</div>
  </div>
  <div>~~~~~~~~复选框绑定~~~~~~~~~</div>
  <div>
    <div>check names：{{ checkNames }}</div>

    <input name="name1" type="checkbox" value="Jack" v-model="checkNames">
    <label for="name1" style="margin-right:10px">Jack</label>

    <input name="name2" type="checkbox" value="Mask" v-model="checkNames">
    <label for="name2" style="margin-right:10px">Mask</label>

    <input name="name3" type="checkbox" value="Amy" v-model="checkNames">
    <label for="name3">Amy</label>
  </div>
  <div>~~~~~~~~选择器绑定~~~~~~~~~</div>
  <div>
    <select v-model="select" style="width:150px;height:25px">
      <option value="A">A</option>
      <option value="B">B</option>
      <option value="C">C</option>
    </select>
    select：{{ select }}
  </div>
</template>