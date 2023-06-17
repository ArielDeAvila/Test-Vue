<script setup>
const currentPath = 'Dashboard/'
</script>

<template>

<div class="breadcrumb hide">
    <p>{{ currentPath }}</p>
</div>

</template>

<style>
.breadcrumb{
    height: 3.28vw;

    text-align: left;
    padding-left: 4.89vw;
    display: flex;
    align-items: center;

    background-color: #2D3339;
}

.breadcrumb p{
    color: var(--background-green);
    margin: 0;
    font-size: 0.83vw;
    font-weight: 600;
}
</style>