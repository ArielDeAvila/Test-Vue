<script setup>
import { ref } from 'vue'

const name = ref('David')
</script>

<template>
    <div class="profile">
        <div class="photo">
            <img src="/profile.png" alt="profile">
        </div>
        <p class="hide">{{ name }}</p>
        <span class="triangle"></span>
    </div>

</template>

<style scoped>
.profile{
    display: flex;
    align-items: center;
    gap: 1.3vw;
    height: 2.92vw;
    width: 9.48vw;
    border: 1px solid var(--background-gray);
    border-radius: 0.63vw;
    padding-right: 0.94vw;
}

.profile p{
    
    color: #fff;
    font-size: 0.83vw;
}

.photo{
    width: 2.92vw;
    height: 2.92vw;
    background-color: #c4c4c4;
    border-radius: 0.63vw;
}

.photo img{
    width: 2.92vw;
    height: 2.92vw;
}

.triangle{
    width: 0;
    height: 0;
    border-top: 0.4vw solid #D3D6E4;
    border-right: 0.4vw solid transparent;
    border-left: 0.4vw solid transparent;

    
}



</style>