<script setup>
import {ref} from 'vue'
const headerTitle = ref('1987 CONSTITUTION OF THE REPUBLIC OF THE PHILIPPINES')
</script>

<template>
    <header>
        <h1>{{ headerTitle }}</h1>
    </header>
</template>

<style scoped>
/*HEADER CSS*/
header img {
  height: 150px;
}

header h1 {
  font-size: 2rem;
  color: #34495e;
  margin-top: 10px;
}
</style>