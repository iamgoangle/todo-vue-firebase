<template>
  <div class="container">
    <h1 v-once>{{ title }}</h1>
    <TodoTable :todos="todos" />
  </div>
</template>

<script>
import TodoTable from './TodoTable';

const todos = [
  { id: 1, isActive: true, symbol: 'GBPUSD', action: 'Buy', entry: 1.3346, tp: 1.40000, sl: 1.3200 },
];

export default {
  name: 'Todo',
  created() {
    // console.log('Component Todo created');
  },
  mounted() {
    // console.log('Component Todo mounted');
  },
  components: { TodoTable },
  data() {
    return {
      title: 'Forex Todo',
      todos,
    };
  },
};
</script>

<style scoped>
  h1 {
    font-weight: normal;
  }
</style>
