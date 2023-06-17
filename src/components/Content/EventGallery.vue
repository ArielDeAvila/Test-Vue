<script>
// import Swiper core and required modules
import { Navigation, Pagination, Scrollbar, A11y } from 'swiper';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

import axios from 'axios';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';
import 'swiper/css/scrollbar';

// Import Swiper styles
export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        const onSwiper = (swiper) => {
            console.log(swiper);
        };
        const onSlideChange = () => {
            console.log('slide change');
        };
        return {
            onSwiper,
            onSlideChange,
            modules: [Navigation, Pagination, Scrollbar, A11y],
        };
    },
    data() {
        return {
            datos: []
        }
    },
    mounted() {
         
        axios.get('https://picsum.photos/v2/list?page=2&limit=100')
            .then(res => {
                this.datos = res.data;
            })
            .catch(err => {
                console.error(err);
            })
        
    }
   
};
</script>

<template>
<div>
    <h1 class="gallery-title">Event Galleries</h1>
    <div class="carrousel">
        <swiper
            :modules="modules"
            :slides-per-view="1"
            :space-between="10"
            navigation
            @swiper="onSwiper"
            @slideChange="onSlideChange"
        
            >
            <swiper-slide v-for="dato in datos" :key="dato.id" class="slide">
                <img :src="dato.download_url" alt="img1" class="img-carrousel">
                <p class="p-slide">{{ dato.author }}</p>
            </swiper-slide>
        </swiper>
    </div>
</div>
</template>



<style scoped>
h1{
    font-size: 1.98vw;
    font-weight: 500;
    text-align: left;
    margin-top: 0;
}

.carrousel{
    width: 45.78vw;
    height: 28.91vw;
    border-radius: 0.89vw;
    overflow: hidden;
    position: relative;
} 

.img-carrousel{
    width: 45.78vw;
    height: 28.91vw;
}

.p-slide{    
    text-align: center;
    background-color: rgba(47, 54, 61, 0.7);
    width: 100%;
    padding: 3.98vh 0;
    margin: 0;
    position: absolute;
    bottom: 0;
    font-size: 1.14vw;
}

.slide{
    position: relative;
}


</style>