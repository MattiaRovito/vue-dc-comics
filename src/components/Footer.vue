<template>
  
  
  <footer>
        
        <div class="footer-top">
           <div class="container">
             <nav>
                <h3 class="uppercase">DC Comics</h3>
                <ul>
                  <li>Characters</li>
                  <li>Comics</li>
                  <li>Movies</li>
                  <li>TV</li>
                  <li>Games</li>
                  <li>Videos</li>
                  <li>News</li>
                </ul>
             </nav>
             <nav>
                <h3 class="uppercase">Shop</h3>
                <ul>
                  <li>Characters</li>
                  <li>Comics</li>
                  
                </ul>
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
          height: 350px;
          position: absolute;
          top: -50px;
          right: 40px;
          z-index: 2;
        }
    }

    nav
    {
      color:white;
      padding: 15px;
     
      h3
      {
         margin-bottom: 15px;
      }

      li
      {
        color: #959595;
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
