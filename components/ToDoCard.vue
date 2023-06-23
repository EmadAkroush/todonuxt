<template>
    <div class=" mt-10 text-red shadow-md p-4 h-full rounded-sm">
        <div class="flex flex-col h-full justify-between">
        <nuxt-link :to="`tododetails/${items.id}`">  <p> {{ items.title }} </p> </nuxt-link>
            <p> {{ items.completed }}</p>
        </div>
    </div>
</template>

<script setup>
  const { items } = defineProps(['items'])
</script>

<style lang="scss" scoped></style>