<template>

<div class="jumbo-space">
    
    <h2 class="series uppercase">Current Series</h2>

</div>
  

</template>






<script>

export default {
  name: 'Jumbotron',

}
</script>


<style lang="scss" scoped>

.jumbo-space
{
    height: 300px;
    background-image: url('../assets/jumbotron.jpg');
    background-size: cover;
    position: relative;

    .series
    {
      color:white;
      padding: 10px 20px;
      background-color: #0282f9;
      width: 18%;
      position: absolute;
      bottom: -15px;
      left: 165px;
    }

}




</style>
