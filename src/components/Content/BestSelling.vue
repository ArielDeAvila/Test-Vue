<template>
<div class="content-chart-percent">
    <div class="title">
        <h2>Best Selling</h2>
        <p>This Week &nbsp;&nbsp;<span class="triangle"></span></p>
    </div>
    <div class="day">
        <p>Tuesday</p>
        <p>215,253 pcs</p>
    </div>
    <div class="chart-content">
        <div class="chart-percent">
            <img src="/pieCharts.svg" alt="pie-chart" class="pie-chart">
        </div>
        <div class="chart-column hide">
            <img src="/chart.svg" alt="bar-chart" class="bar-chart">
        </div>
    </div>
</div>

</template>

<style scoped>
.content-chart-percent{
    background-color: var(--background-content);
    border-radius: 0.89vw;
    width: 43.86vw;
    padding: 1.79vw;
}

.title{
    display: flex;
    justify-content: space-between;
    align-items: baseline;
}

.title h2{
    font-family: 'Poppins';
    font-size: 1.3vw;
    font-weight: 500;
    line-height: 37px;
    letter-spacing: 0em;
    text-align: left;

    margin-top: 0;
}

.title p{
    display: flex;
    align-items: center;
    font-size: 0.77vw;
}

.triangle{
    width: 0;
    height: 0;
    border-top: 0.4vw solid #D3D6E4;
    border-right: 0.4vw solid transparent;
    border-left: 0.4vw solid transparent;  
}

.day{
    background-color: #20262D;
    padding: 0.92vw 1.66vw ;
    display: flex;
    justify-content: space-between;
    border-radius: 0.89vw;
}

.day p{
    margin: 0;
    font-size: 0.89vw;
}

.chart-content{
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    flex-wrap: wrap;
}


.bar-chart{
    width: 16.85vw;
}

.pie-chart{
    width: 23.37vw;
}
</style>