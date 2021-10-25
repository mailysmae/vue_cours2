<template>
  <div>
    VTodoItem
  </div>
</template>

<script>
export default {
  setup () {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.v-todo-item {
  padding: 8px;
  display: flex;
  justify-content: space-between;
  background: white;
  border-radius: 3px;
  background: antiquewhite;

  &.is-checked {
    filter: grayscale(1);

    span {
      text-decoration: line-through;
    }
  }
}
</style>
