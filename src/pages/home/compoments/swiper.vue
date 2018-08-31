<template>
    <div class="swiper">
        <swiper :options="swiperOption">
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgurl" />
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>   
    </div>
    
</template>
<script>
export default{
    name:'HomeSwiper',
    data:function(){
        return{
            swiperOption:{
                pagination:'.swiper-pagination',
                loop:true
            },
            swiperList:[{
                id:'0001',
                imgurl:'https://aecpm.alicdn.com/simba/img/TB1CWf9KpXXXXbuXpXXSutbFXXX.jpg_q50.jpg'
            },{
                id:'0002',
                imgurl:'https://aecpm.alicdn.com/simba/img/TB14ab1KpXXXXclXFXXSutbFXXX.jpg_q50.jpg'
            },{
                id:'0003',
                imgurl:'//gw.alicdn.com/imgextra/i3/156/TB2Cvb.ubsrBKNjSZFpXXcXhFXa_!!156-0-lubanu.jpg'
            }]
        }
    }
}
</script>
<style lang='stylus' scoped>
    .swiper >>> .swiper-pagination-bullet-active
        background:#fff
    .swiper
        overflow:hidden
        width:100%
        height:0
        padding-bottom:31.25%
        background:#eee
        .swiper-img
            width:100%
</style>