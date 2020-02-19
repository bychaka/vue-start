<template>
    <div>
        <ul>
            <TodoItem
                v-for="todo of todos"
                :todo="todo"
                :key="todo.id"
            />
        </ul>
    </div>
</template>

<script>
    import TodoItem from '@/components/TodoItem'
    export default {
        props: ['todos'],
        components: {
            TodoItem
        }
    }
</script>

<style scoped>
    ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
    }
</style>