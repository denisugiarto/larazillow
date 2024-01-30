<template>
    <Link href="/listing">Listings</Link>&nbsp;
    <Link href="/listing/create">New Listing</Link>
    <!-- <div>The Page with time {{ timer }}</div> -->
    <div v-if="flashSuccess" class="success">
        {{ flashSuccess }}
    </div>
    <!-- <div>{{ y }}</div> -->
    <!-- <p>{{ JSON.stringify(page, null, 2) }}</p> -->
    <slot>Default</slot>
</template>
<script setup>
import { computed, ref } from "vue";
import { Link, usePage } from "@inertiajs/vue3";
// import { ref } from "vue";
const page = usePage();
const flashSuccess = computed(() => page.props.flash.success);
// const timer = ref(0);
// const x = ref(0);
// const y = computed(() => x.value * 2);

// setInterval(() => timer.value++, 1000);
</script>

<style scoped>
.success {
    background-color: green;
    color: white;
}
</style>
