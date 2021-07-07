<template>
  
  
  <footer>
        
        
           <div class="footer-top" >
             <div class="container">
              <nav >
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
        

        <div class="footer-bottom clearfix">
            <div class="container">
              <h3 class="uppercase">Sign-Up Now!</h3>
              <img class="float-right padding" src="@/assets/footer-facebook.png" alt="">
              <img class="float-right padding" src="@/assets/footer-twitter.png" alt="">
              <img class="float-right padding" src="@/assets/footer-youtube.png" alt="">
              <img class="float-right padding" src="@/assets/footer-pinterest.png" alt="">
              <img class="float-right padding" src="@/assets/footer-periscope.png" alt="">
              <h2 class="uppercase float-right">Follow Us</h2>
             
            </div>
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
  position: relative;


    
    .logo-dx
    {
        position: absolute; 
        top: -50px;
        right: 40px;
        
        img
        {
          height: 350px;
          
          
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
  padding: 25px;

  .clearfix::after {
    content: "";
    clear: both;
    display: table;
  }

  h3
  {
    color: white;
    padding: 10px 20px;
    border: 2px solid #0282f9;
    width: 17%;
    display: inline-block;
    
  }

  h2
  {
    color: #0282f9;
    margin-right: 10px;
    line-height: 45px;
  }

}

.float-right
{
  float:right;
}

.float-left
{
  float:left;
}

.padding
{
  // margin: 10px;
  padding: 5px;
}



</style>
