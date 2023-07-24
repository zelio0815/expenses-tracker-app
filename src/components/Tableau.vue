<script setup>
import Badge from './Badge.vue';
import ActionButton from './ActionButton.vue';


</script>

<template>
    <table class="table table-bordered text-center">
        <thead class="table-dark">
            <tr>
                <th scope="col">#</th>
                <th scope="col">Title</th>
                <th scope="col">Amount</th>
                <th scope="col">Type</th>
                <th scope="col">Actions</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row">1</th>
                <td>FreeLance</td>
                <td>500</td>
                <td>
                    <Badge badgeClass="btn btn-success">
                        <template #titre>Deposit</template>
                    </Badge>
                </td>
                <td>
                    <ActionButton actionButtonClass="btn btn-outline-primary" class="me-2">
                        <template #titre><i class="bi bi-pencil-square"></i> Modify</template>
                    </ActionButton>
                    <ActionButton actionButtonClass="btn btn-outline-danger">
                        <template #titre><i class="bi bi-trash-fill"></i> Delete</template>
                    </ActionButton>
                </td>
            </tr>
            <tr>
                <th scope="row">2</th>
                <td>Trading</td>
                <td>9000</td>
                <td>
                    <Badge badgeClass="btn btn-success">
                        <template #titre>Deposit</template>
                    </Badge>
                </td>
                <td>
                    <ActionButton actionButtonClass="btn btn-outline-primary" class="me-2">
                        <template #titre><i class="bi bi-pencil-square"></i> Modify</template>
                    </ActionButton>
                    <ActionButton actionButtonClass="btn btn-outline-danger">
                        <template #titre><i class="bi bi-trash-fill"></i> Delete</template>
                    </ActionButton>
                </td>
            </tr>
            <tr>
                <th scope="row">3</th>
                <td>Trading</td>
                <td>500</td>
                <td>
                    <Badge badgeClass="btn btn-danger">
                        <template #titre>Expense</template>
                    </Badge>
                </td>
                <td>
                    <ActionButton actionButtonClass="btn btn-outline-primary" class="me-2">
                        <template #titre><i class="bi bi-pencil-square"></i> Modify</template>
                    </ActionButton>
                    <ActionButton actionButtonClass="btn btn-outline-danger">
                        <template #titre><i class="bi bi-trash-fill"></i> Delete</template>
                    </ActionButton>
                </td>
            </tr>
            <tr>
                <th scope="row">4</th>
                <td>Rent</td>
                <td>2500</td>
                <td>
                    <Badge badgeClass="btn btn-danger">
                        <template #titre>Expense</template>
                    </Badge>
                </td>
                <td>
                    <ActionButton actionButtonClass="btn btn-outline-primary" class="me-2">
                        <template #titre><i class="bi bi-pencil-square"></i> Modify</template>
                    </ActionButton>
                    <ActionButton actionButtonClass="btn btn-outline-danger">
                        <template #titre><i class="bi bi-trash-fill"></i> Delete</template>
                    </ActionButton>
                </td>
            </tr>
            <tr>
                <th scope="row">5</th>
                <td>Foods</td>
                <td>500</td>
                <td>
                    <Badge badgeClass="btn btn-danger">
                        <template #titre>Expense</template>
                    </Badge>
                </td>
                <td>
                    <ActionButton actionButtonClass="btn btn-outline-primary" class="me-2">
                        <template #titre><i class="bi bi-pencil-square"></i> Modify</template>
                    </ActionButton>
                    <ActionButton actionButtonClass="btn btn-outline-danger">
                        <template #titre><i class="bi bi-trash-fill"></i> Delete</template>
                    </ActionButton>
                </td>
            </tr>
        </tbody>
    </table>
</template>

<style lang="scss" scoped></style>