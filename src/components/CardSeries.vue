<script>
export default {
    props:{
        serie: Object,
    }
}
</script>
<template lang="">
    <div class="card">
        <div class="card-image">
            <img :src="serie.thumb" alt="image">
            <h4>{{serie.series}}</h4>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    .card{
        width: 15%;
        padding: 10px;
        img{
            width: 80%;
        }
    }
</style>