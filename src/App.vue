<script setup lang="ts">
import axios from 'axios';
import { onMounted } from 'vue';

onMounted(() => {
    axios
        .get('https://devapi.qweather.com/v7/weather/now', {
            params: {
                key: 'c42a982f075a47c192e0db18cc805a6a',
                location: '101010100',
            },
        })
        .then(res => {
            console.log(res.data);
        });
});
</script>

<template></template>

<style></style>
