<script setup>
defineProps({
    actionButtonClass: String,
})
</script>

<template>
    <button type="button" :class="actionButtonClass" class="px-2 rounded">
        <slot name="titre"></slot>
    </button>
</template>

<style lang="scss" scoped></style>