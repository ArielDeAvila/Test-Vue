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
    <div class="notification" :class="{newNotification: hasNewNotication}" @click="toggleButton">
        <img src="/notification.png" alt="settings" >
    </div>
</template>

<style>
    .notification{
        width: 2.92vw;
        height: 2.92vw;
        border-radius: 0.63vw;

        display: inline-flex;
        align-items: center;
        justify-content: center;
        
        background-color: var(--background-gray);

        position: relative;
    }

    .notification img{
        height: 1.46vw;
        width: 1.46vw;
    }

    .newNotification::before{
        content: '';
        background-color: #D9B75F;

        width: 0.83vw;
        height: 0.83vw;

        border-radius: 0.83vw;

        position: absolute;
        top: -0.16vw;
        right: -0.16vw;
        
    }
</style>