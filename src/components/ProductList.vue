<script setup>
import productlist from '@/assets/productos.json'
import { RouterLink } from 'vue-router';
</script>

<template>
    <ul>
        <li v-for="product in productlist" :key="product.id">
            <RouterLink :to="'/productdetail/' + product.id">{{ product.name }}</RouterLink>
        </li>
    </ul>

</template>

<style scoped>
    ul {
        display: flex;
        flex-direction: column;
        gap: 3px;
    }

    li {
        color: black;
    }
</style>