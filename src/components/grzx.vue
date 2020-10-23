<template>
    <div>
        <div class="grzx-up">
            当前位置：<span class="grzx-up">个人中心</span>
        </div>
        <div class="grzx-down" v-for="(item,index) in grzxList" :key="index">
            <img :src="item.url" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name:'grzx',
    data(){
        return{
        grzxList:this.getGrzxList(),
        }
    },
    methods:{
        getGrzxList(){
            return[
                {
                    id:0,
                    url:require('@/assets/image/grzx1.png')
                },
                {
                    id:1,
                    url:require('@/assets/image/grzx2.png')
                },
                {
                    id:2,
                    url:require('@/assets/image/grzx3.png')
                },
                {
                    id:3,
                    url:require('@/assets/image/grzx4.png')
                },
                {
                    id:4,
                    url:require('@/assets/image/grzx5.png')
                },
            ]
        }
    }
}
</script>

<style lang='less'>

</style>