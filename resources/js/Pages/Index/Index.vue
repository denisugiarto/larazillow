<template>
    <MainLayout>
        <h1>Index</h1>
        <div>The message is {{ message }}</div>
    </MainLayout>
</template>

<script setup>
import MainLayout from "../../Layouts/MainLayout.vue";
defineProps({
    message: String,
});
</script>
