<script setup>
import productlist from '@/assets/productos.json'

</script>

<template>
    <div>
        <h1>Product Detail</h1>
        <p>{{ $route.params.id }}</p>
    </div>
</template>