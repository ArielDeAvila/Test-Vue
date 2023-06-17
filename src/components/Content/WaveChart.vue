<template>

<div class="content-wave-chart content-charts">
    <div class="info-wave">
        <div>
            <h2>451,509</h2>
            <p>This Week &nbsp;&nbsp;<span class="triangle"></span></p>
        </div>

        <p>Sales</p>
    </div>
    <img src="/wave.svg" alt="wave" class="wave">
</div>

</template>

<style scoped>
.content-wave-chart{
    overflow: hidden;

    position: relative;
}


.info-wave div{
    display: flex;
    justify-content: space-between;
}

.info-wave div p{
    display: flex;
    align-items: center;
}

.info-wave p{
    margin: 0;
    font-size: 0.77vw;
}

.info-wave h2{
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

.wave{
    
    height: 11vw;
    
    position: absolute;
    top: 0;
    left: 0;

}

</style>