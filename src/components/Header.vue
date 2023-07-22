<script setup>
</script>

<template>
    <header class="p-4">
        <nav class="container text-light expense-header d-flex flex-row justify-content-between align-items-center">
            <div class="d-flex flex-row justify-content-between align-items-center expense-title">
                <p class="mb-0"><i class="bi bi-bank display-6"></i></p>
                <p class="ms-4 display-6 fw-normal mb-0">Banking App</p>
            </div>
            <div class="d-flex flex-row justify-content-between align-items-center">
                <RouterLink :to="{ name: 'home' }" class="expense-route display-6 fw-light me-4">Home</RouterLink>
                <RouterLink :to="{ name: 'stats' }" class="expense-route display-6 fw-light">Stats</RouterLink>
            </div>
        </nav>
    </header>
</template>

<style scoped>
.expense-route {
    text-decoration: none;
    color: inherit;
    opacity: 0.5;
}

/* .expense-title {
    cursor: pointer;
} */

a.router-link-active {
    opacity: 1;
}

header {
    background-color: #331D2C;
}
</style>