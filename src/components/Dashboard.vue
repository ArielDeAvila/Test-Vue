<script setup>
import BestSelling from './Content/BestSelling.vue'
import ProgressBar from './Content/progressBarChart.vue'
import WaveChart from './Content/WaveChart.vue'
import WaveLineChart from './Content/WaveLineChart.vue'
import PieChart from './Content/PieChart.vue'
import BarChart from './Content/BarChart.vue'
import EventGallery from './Content/EventGallery.vue'
</script>

<template>
    <div class="content">
        <div class="left">
            <BestSelling/>
            <div class="group-charts">
                <ProgressBar/>
                <WaveChart/>
                <WaveLineChart/>
                <PieChart/>
            </div>
        </div>
        <div class="right">
            <BarChart/>
            <EventGallery/>
        </div>
    </div>
</template>

<style >
    .content{
        background-color: var(--background-black);
        padding: 2.45vw 1.72vw 3.25vw 1.72vw;
        display: grid;
        grid-template-columns: auto auto;
        column-gap: 2.3vw;
        
    }

    .left{
        display: flex;
        flex-direction: column;
        gap: 1.67vw;
    }

    .group-charts{
        display: grid;
        grid-template-columns: auto auto;
        row-gap: 1.7vw;
        column-gap: 1.7vw;
        
    }

    .content-charts{
        background-color: var(--background-charts);
        width: 19.11vw;
        height: 6.55vw;
        padding: 1.39vw 1.95vw 1.66vw 1.56vw;    
        border-radius: 0.89vw;
    }

    .content-charts > p{
        font-size: 0.77vw;
    }

    .content-charts h2{
        font-size: 1.02vw;
    }

    .right{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

</style>