<template>
    <div class="app">
        <router-view></router-view>
        <app-footer></app-footer>
    </div>
</template>

<script>
    import TodoList from 'todoList.vue'
    import Blocks from  'blocks.vue'
    import AppHeader from 'components/appHeader.vue'
    import TaskList from 'components/taskList.vue'
    import AppFooter from 'components/appFooter.vue'

    export default {
        name: 'app',
        data() {
            return {
                msg: 'Hello, Vue-loader'
            }
        },
        components: {
            "todo-list": TodoList,
            "blocks": Blocks,
            "app-header": AppHeader,
            "task-list": TaskList,
            "app-footer": AppFooter
        }
    }
</script>

<style>
    .message {
        color: red;
    }
</style>