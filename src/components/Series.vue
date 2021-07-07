<template>

    <div class="container">
        
        <div class="current-series clearfix">
            <img class="img" :src="prod.thumb" :alt="prod.series">
            <!-- <p>{{prod.series}}</p> -->
        </div>
        
    </div>
 
</template>

<script>
export default {
    name: 'Series',
    props: ["prod"]
}
</script>

<style lang="scss" scoped>


.current-series
{

    .clearfix::after 
    {
        content: "";
        clear: both;
        display: table;
    }


    .img
    {
        display:block;
        float: left;
        width: 15%;
        padding: 20px;
    }

   
}
p
{
    color: white;
    // display: block;
}



</style>