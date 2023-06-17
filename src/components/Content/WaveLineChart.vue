<template>

    <div class="content-wave-line content-charts hide">
        <div class="info-line">
            <div>
                <h2>$456,623</h2>
                <p>Monthly &nbsp;&nbsp;<span class="triangle"></span></p>
            </div>

            <p>Income</p>
        </div>
        <img src="/wave-line.svg" alt="wave-line" class="wave-line">
    </div>
</template>

<style scoped>
.content-wave-line{
    overflow: hidden;

    position: relative;
}

.info-line div{
    display: flex;
    justify-content: space-between;
}

.info-line div p{
    display: flex;
    align-items: center;
}

.info-line p{
    margin: 0;
    font-size: 0.77vw;
}

.info-line h2{
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

.wave-line{
   
    height: 11.5vw;

    position: absolute;
    top: 0;
    left: -1.5vw;
}

</style>