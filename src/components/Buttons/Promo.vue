<script>
export default {
    data() {
        return {
            notification: 1,
            hasNewNotication: true
        };
    },
    methods: {
        toggleButton() {
            this.notification = this.notification - 1;
            this.hasNewNotication = this.notification > 1
        }
    }
}
</script>

<template>
    <div class="promo hide" :class="{ newNotificationPromo: hasNewNotication }" @click="toggleButton">
        <img src="/promo.png" alt="settings" height="24">
    </div>
</template>

<style>
.promo {
    width: 2.92vw;
    height: 2.92vw;
    border-radius: 0.63vw;

    display: inline-flex;
    align-items: center;
    justify-content: center;

    background-color: var(--background-gray);

    position: relative;
}

.promo img{
    height: 1.46vw;
    width: 1.46vw;
}

.newNotificationPromo::before{
    content: '';
    background-color: #647280;

    width: 0.83vw;
    height: 0.83vw;

    border-radius: 0.83vw;

    position: absolute;
    top: -0.16vw;
    right: -0.16vw;
    
}
</style>