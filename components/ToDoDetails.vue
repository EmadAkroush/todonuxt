<template>
    <div class="p-20">
        <p>    {{ details.title }}  </p>
        <p>    {{ details.completed }}  </p>
    </div>
</template>

<script setup>
  const { details } = defineProps(['details'])
</script>

<style lang="scss" scoped>

</style>