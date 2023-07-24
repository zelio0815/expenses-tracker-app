<script setup>
defineProps({
    badgeClass: String,
})
</script>

<template>
    <button type="button" :class="badgeClass" class="px-2 rounded" style="pointer-events: none;">
        <slot name="titre"></slot>
    </button>
</template>

<style lang="scss" scoped></style>