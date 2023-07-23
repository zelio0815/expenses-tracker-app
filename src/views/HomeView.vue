<script setup>
import Formulaire from '../components/Formulaire.vue';

</script>

<template>
    <form class="container d-flex flex-column align-items-start mt-2">
        <Formulaire fieldSetClass="border border-success" buttonClass="btn btn-outline-success" legendClass="text-success">
            <template #legende>Deposit</template>
            <template #titre>Deposit</template>
            <template #amount>Amount</template>
            <template #boutton>Add Deposit</template>
        </Formulaire>
        <Formulaire fieldSetClass="border border-danger" buttonClass="btn btn-outline-danger" legendClass="text-danger">
            <template #legende>Expense</template>
            <template #titre>Expense</template>
            <template #amount>Amount</template>
            <template #boutton>Add Expense</template>
        </Formulaire>
    </form>
</template>

<style lang="scss" scoped>
</style>