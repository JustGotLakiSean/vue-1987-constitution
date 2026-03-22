<script setup>
import {ref} from 'vue';
const copyrightYear = ref('2026')
const href = ref('#')
</script>

<template>
    <footer>
        Copyright &copy; {{ copyrightYear }}<a :href>HOME</a>
    </footer>
</template>

<style scoped>

</style>