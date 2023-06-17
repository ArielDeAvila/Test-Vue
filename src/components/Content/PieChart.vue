<template>

    <div class="content-pie-chart content-charts">

        <div class="pie">
            <img src="/pie.svg" alt="pie" class="img-pie">
        </div>
        <div class="info-pie hide">
            <p>This Week &nbsp;&nbsp;<span class="triangle"></span></p>
        </div>
        <div class="legend hide">
            <img src="/legends.svg" alt="legends" class="img-legends">
        </div>



    </div>
</template>

<style scoped>
.content-pie-chart{
    

    display: grid;
    grid-template-columns: auto auto;
    align-items: end;
    justify-content: space-between;
}

.pie{
  

    grid-column: 1;
    grid-row: 1 / span 2;
}

.img-pie{
    width: 6.19vw;
    height: 6.30vw;
}

.img-legends{
    width: 11.18vw;
    height: 3.56vw;
}

.info-pie p{
    display: flex;
    align-items: center;
    justify-content: flex-end;
    margin: 0;
    font-size: 0.77vw;
}

.triangle{
    width: 0;
    height: 0;
    border-top: 0.4vw solid #D3D6E4;
    border-right: 0.4vw solid transparent;
    border-left: 0.4vw solid transparent;  
}
</style>