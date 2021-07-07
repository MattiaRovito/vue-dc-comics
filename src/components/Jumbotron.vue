<template>

<div class="jumbo-space">
    
    <a href="#">
      <h2 class="series uppercase">Current Series</h2>
    </a>

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
      bottom: -18px;
      left: 165px;
      z-index: 20;
    }

}




</style>
