<template>
    <div>
        <div>
            <home-header></home-header>
            <home-swiper></home-swiper>
        </div>   
    </div>
    
</template>

<script>
import HomeHeader from './compoments/Header'
import HomeSwiper from './compoments/swiper'
export default{
    name:'home',
    components:{
        HomeHeader:HomeHeader,
        HomeSwiper:HomeSwiper
    }
}
</script>

<style>
    
</style>