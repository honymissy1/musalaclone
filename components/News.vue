<template>
    <div class="header">
        <h1>Musala Soft <span style="color: steelblue">News</span></h1>
    </div>

    <div>
        <Swiper :modules="[Navigation]"
                loop
                :breakpoints="{
                    '1000': {
                    slidesPerView:'2'
                  }
                }"
                :slides-per-view="1"
                :autoplay="{
                delay: 1000,
                disableOnInteraction: false,
                }"
                :space-between="100"
                :navigation="true"
                > 
            <SwiperSlide>
                <div class="splide">
                    <img src="../assets/images/card1.jpg" alt="">
                    <div style="padding: 10px;">
                        <h1>Qinshift the new brand of musala softs mother company</h1>
                        <p>Over the last six years, the KKCG technology pillar has grown to become a leading European 
                            IT player with annual revenues of nearly EUR 500 million,
                             employing more than 4,000 experts across 13 companies. Now it consolidates its position
                             as an international Information Technology (IT) leader.
                        </p>
                    </div>

                    <p style="text-align: right; color: brown; padding: 5px">10 Jan 2023</p>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="splide">
                    <img src="../assets/images/card2.jpg" alt="">
                    <div style="padding: 10px;">
                        <h1>23 Years CodeIT</h1>
                        <p>Over the last six years, the KKCG technology pillar has grown to become a leading European 
                            IT player with annual revenues of nearly EUR 500 million,
                             employing more than 4,000 experts across 13 companies. Now it consolidates its position
                             as an international Information Technology (IT) leader.
                        </p>
                    </div>
                    <p style="text-align: right; color: brown; padding: 5px">10 Jan 2023</p>
                </div>
            </SwiperSlide>

            <SwiperSlide>
                <div class="splide">
                    <img src="../assets/images/card3.jpg" alt="">
                    <div style="padding: 10px;">
                        <h1>Musala Soft Opens it's office in Cairo</h1>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo minima dolor necessitatibus, 
                            fugit quos maiores nobis placeat temporibus cumque modi neque eligendi ducimus numquam obcaecati
                             praesentium, sed at beatae, minus laborum impedit vero?
                        </p>
                        
                    </div>
                    <p style="text-align: right; color: brown; padding: 5px">10 Jan 2023</p>
                </div>
            </SwiperSlide>

        </Swiper>

    </div>
</template>

<script setup>
    
 import { Swiper, SwiperSlide } from 'swiper/vue';
 import { Navigation, Pagination, Autoplay, A11y, EffectCards } from 'swiper/modules';

 import 'swiper/css';
  import 'swiper/css/navigation';
  import 'swiper/css/pagination';
  import 'swiper/css/scrollbar';
  import 'swiper/css/autoplay'

  
</script>

<style scoped>
.header h1{
  text-align: center;
  font-size: 30px;
  color: rgba(0, 0, 0, 0.852);
  margin-top: 30px;
}

.swiper{
    min-width: 300px;
    width: 70%;
    height: auto;
    /* border: 1px solid; */
    margin-bottom: 50px;
}

.swiper-button-prev, .swiper-button-next{
    color: black;
    font-size: 50px;
    background-color: black;
}

.splide{
    /* border: 1px solid; */
    height: 100%
}

.splide img{
    width: 100%
}

.splide h1{
    font-size: 20px;
}

</style>