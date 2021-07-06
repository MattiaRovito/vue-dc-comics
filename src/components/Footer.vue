<template>
  
  
  <footer>
        
        <div class="footer-top">
           <div class="container">
             <nav>

             </nav>

             <div class="logo-dx">
               <img src="../assets/dc-logo-bg.png" alt="DC logo bg">
             </div>
           </div>
        </div>
        

        <div class="footer-bottom">
            
        </div>

    </footer>


</template>




<script>
export default {
  name: 'Footer',
 
}
</script>



<style lang="scss" scoped>


.footer-top
{
  background-image: url(../assets/footer-bg.jpg);
  height: 300px;
  z-index: 3;
    
    .logo-dx
    {
        position: relative;

        img
        {
          height: 400px;
          position: absolute;
          top: -50px;
          right: 40px;
          z-index: 2;
        }
    }
}

.footer-bottom
{
  height: 90px;
  background-color: #303030;
  z-index: 300;
}




</style>
