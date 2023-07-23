<script setup>
defineProps({
  fieldSetClass: String,
  buttonClass: String,
  legendClass: String
})
</script>

<template>
  <fieldset id="conteneur" :class="fieldSetClass" class="rounded p-4 m-4">
    <legend class="fw-bold" :class="legendClass">
      <slot name="legende"></slot>
    </legend>
    <div class="form-floating pb-3">
      <input type="text" class="form-control" id="titre" placeholder="titre">
      <label for="titre">
        <slot name="titre"></slot>
      </label>
    </div>
    <div class="form-floating pb-3">
      <input type="number" class="form-control" id="amount" placeholder="amount">
      <label for="amount">
        <slot name="amount"></slot>
      </label>
    </div>
    <button type="button" :class="buttonClass" class="px-4 py-2">
      <slot name="boutton"></slot>
    </button>
  </fieldset>
</template>

<style scoped>
#conteneur {
  width: 400px;
}
</style>