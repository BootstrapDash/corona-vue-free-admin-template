<template>
  <section class="todo">
    <div class="row">
      <div class="col-lg-12">
        <div class="card">
          <div class="card-body">
            <h4 class="card-title">Todo list</h4>
            <todo-list />
          </div>
        </div>
      </div>
    </div>
  </section> 
</template>

<script>
import todoList from '../../components/apps/todoList'
export default {
  name: 'todo',
  components: {
    todoList
  }
}
</script>