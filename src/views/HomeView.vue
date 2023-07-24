<script setup>
import Card from '../components/Card.vue';
import Formulaire from '../components/Formulaire.vue';
import Tableau from '../components/Tableau.vue'

</script>

<template>
    <div class="container d-flex justify-content-around">
        <form class="d-flex flex-column align-items-start mt-2">
            <Formulaire fieldSetClass="border border-success" buttonClass="btn btn-outline-success"
                legendClass="text-success">
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
        <div class="d-flex flex-column border mt-2 p-4 align-items-center" style="width: 60%;">
            <div class="d-flex mb-4 align-items-center" style="height: 50%;">
                <Card cardClass="border-success text-success">
                    <template #titre>DEPOSITS</template>
                    <template #logo><i class="bi bi-cash-stack"></i></template>
                    <template #valeur>0</template>
                </Card>
                <Card cardClass="border-danger text-danger mx-4">
                    <template #titre>EXPENSES</template>
                    <template #logo><i class="bi bi-credit-card"></i></template>
                    <template #valeur>0</template>
                </Card>
                <Card cardClass="border-primary text-primary">
                    <template #titre>BALANCE</template>
                    <template #logo><i class="bi bi-currency-dollar"></i></template>
                    <template #valeur>0</template>
                </Card>
            </div>
            <Tableau></Tableau>
        </div>
    </div>
</template>

<style lang="scss" scoped></style>