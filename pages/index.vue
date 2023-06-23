<template>
    <div>
        <div class="grid grid-cols-4 gap-8 p-20 ">
            <div v-for="item in todos" :key="item.id"  >
             <ToDoCard :items="item" />
            </div>
        </div>
    </div>
</template>

<script setup>

const { data: todos } = await useFetch('https://jsonplaceholder.typicode.com/todos')
</script>

<style lang="scss" scoped></style>