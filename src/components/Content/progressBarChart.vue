<template>
<div class="content-progress-bar content-charts">
    <div class="info-bar">
        <div>
            <h2>456k Pcs</h2>
            <p>Daily &nbsp;&nbsp;<span class="triangle"></span></p>
        </div>

        <p>Ticket Sold</p>
    </div>
    <div class="bar">
        <div class="progress-bar"></div>
    </div>
</div>

</template>

<style scoped>
.content-progress-bar{
    

    display: flex;
    flex-direction: column;
    justify-content: space-between;

}

.info-bar div{
    display: flex;
    justify-content: space-between;
}

.info-bar div p{
    display: flex;
    align-items: center;
}

.info-bar p{
    margin: 0;
    font-size: 0.77vw;
}

.info-bar h2{
    margin: 0;
    font-size: 1.02vw;
}

.triangle{
    width: 0;
    height: 0;
    border-top: 0.4vw solid #D3D6E4;
    border-right: 0.4vw solid transparent;
    border-left: 0.4vw solid transparent;  
}

.progress-bar{
    position: relative;
    height: 0.64vw;
    background-color: rgba(255, 255, 255, 0.12);;
    border-radius: 2.49vw;
    
}

.progress-bar::before{
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    border-radius: 2.49vw;
    background-color: var(--bar-color);
    box-shadow: 0 0 1.2vw  rgba(19, 180, 151, 0.56);
    transform: scaleX(0);
    transform-origin: left;
    animation: fill-bar 0.8s 0.3s ease-in-out forwards;
}

@keyframes fill-bar {
    to{
        border-radius: 2.49vw;
        transform: scaleX(var(--fill-size));
        box-shadow: 0 0 1.2vw  rgba(19, 180, 151, 0.56);
    }
}
</style>