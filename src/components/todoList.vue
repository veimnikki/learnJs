<template>
    <div>
        <ul>
            <todoItem 
                v-for="todo in todos" :key="todo"
                v-bind:todo="todo"
            />
        </ul>
    </div>
</template>

<script>
import todoItem from '@/components/todoItem'
export default {
    props: ['todos'],
    components: {
        todoItem
    }
}
</script>