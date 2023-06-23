<template>
    <div>
        <ToDoDetails :details="todos"/>
    </div>
</template>
 
<script setup>
const {id} = useRoute().params
const { data: todos } = await useFetch(`https://jsonplaceholder.typicode.com/todos/${id}`)
</script>



<style lang="scss" scoped>

</style>