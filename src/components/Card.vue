<script setup>
defineProps({
  cardClass: String,
})
</script>

<template>
    <div class="card text-center px-4" :class="cardClass">
        <div class="card-body">
            <legend class="card-title fw-bolder">
                <slot name="titre"></slot>
            </legend>
            <p class="card-text display-1">
                <slot name="logo"></slot>
            </p>
            <legend class="card-text fw-bolder">
                $ <slot name="valeur"></slot>
            </legend>
        </div>
    </div>
</template>

<style lang="scss" scoped></style>
