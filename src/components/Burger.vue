<script>
export default {
    data() {
        return {
            isActive: false
        };
    },
    methods: {
        toggleBurger() {
            this.isActive = !this.isActive
        }
    }
}
</script>

<template>

    <div class="burger" :class="{ active: isActive }" @click="toggleBurger">
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
    </div>
</template>

<style scoped>
.burger {

    margin-right: 0.78vw;
    padding: 0.52vw;
    height: 1.35vw;
    width: 1.35vw;
    border-radius: 8px;

    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
}

.line{
    background-color: white;
    height: 2px;
    width: 100%;
    border-radius: 3px;
    transition: 0.5s;
}

.active .line:nth-child(1){
    transform: translateY(1.5vw) 
    rotate(135deg); 
}

.active .line:nth-child(2){
    transform: scale(0);
}

.active .line:nth-child(3){
    transform: translateY(-1.5vw) rotate(-135deg);
}
</style>