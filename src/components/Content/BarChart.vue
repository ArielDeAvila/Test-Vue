<template>

<div class="content-barchart hide">
    <div class="title-barchart">
        <div>
            <h3>Sales comparasion</h3>
            <p>Than last day</p>
        </div>
        <h1>94%</h1>
    </div>
    <img src="/bar-chart.svg" alt="bar-chart">
</div>
</template>

<style scoped>
.content-barchart{
    width: 45.78vw;
    height: 19.85vw;
    border-radius: 0.89vw;
    background: linear-gradient(113.24deg, #13B497, 16.01%, #05737A 106.71%);
}

.content-barchart img{
    width: 44.05vw;
    height: 13.36vw;
}

.title-barchart{
    padding: 2.17vw 5.44vw 0 2.62vw ;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.title-barchart p, .title-barchart h3{
    margin: 0;
    font-size: 1.28vw;
}

.title-barchart h1{
    font-size: 2.55vw;
    font-weight: 600;
    text-align: left;
    margin: 0;

}

</style>