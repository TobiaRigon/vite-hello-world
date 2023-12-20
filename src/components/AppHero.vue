<script setup>
import { ref } from 'vue'

defineProps({
    title: String,
    description: String,
    logo: String,
})

const count = ref(0)
</script>

<template>
    <div class="jumbotron">
        <img :src="logo" alt="Logo" class="logo" />
    </div>
</template>

<style scoped>
.jumbotron {
    color: antiquewhite;
    padding: 50px;
    background-color: #000000;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    text-align: center;
}

.logo {
    max-width: 100px;
}
</style>
