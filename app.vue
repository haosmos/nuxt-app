<!--
<template>
  <div>
    &lt;!&ndash;    <NuxtWelcome />&ndash;&gt;
    <h1>Hello from Nuxt.js!~~</h1>
    <button @click="fetchTodoList">
      fetch data!
    </button>
    &lt;!&ndash;    <pre>&ndash;&gt;
    &lt;!&ndash;      {{todoList}}&ndash;&gt;
    &lt;!&ndash;    </pre>&ndash;&gt;

    <ul>
      <li v-for="todo in todoList" :key="`todo-id-${todo.id}`">
        <input :checked="todo.completed" type="checkbox">
        {{ todo.title }}
      </li>
    </ul>

  </div>
</template>

<script>
import { defineNuxtComponent } from '#app';

export default defineNuxtComponent({
  data: () => ({
    todoList: []
  }),
  methods: {
    fetchTodoList() {
      fetch('https://jsonplaceholder.typicode.com/todos')
        .then(response =>
          response.json())
        .then(json => {
          this.todoList = json;
        });
    }
  }
});
</script>
-->

<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
