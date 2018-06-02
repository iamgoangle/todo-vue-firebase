<template>
  <div class="row">
    <table class="table table-hover table-dark">
      <thead>
        <tr>
          <th scope="col">isActive</th>
          <th scope="col">Symbol</th>
          <th scope="col">Action</th>
          <th scope="col">Entry</th>
          <th scope="col">TP</th>
          <th scope="col">SL</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="todo in todos" :key="todo.id">
          <th scope="row">{{ todo.isActive }}</th>
          <td>{{ todo.symbol }}</td>
          <td>{{ todo.action }}</td>
          <td>{{ todo.entry }}</td>
          <td>{{ todo.tp }}</td>
          <td>{{ todo.sl }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'TodoTable',
  created() {
    // console.log('Component TodoTable created');
  },
  mounted() {
    // console.log('Component TodoTable mounted');
  },
  props: ['todos'],
};
</script>

<style scoped>
</style>
