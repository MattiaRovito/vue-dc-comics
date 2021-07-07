<template>

  <div class="container header">
      
        <img src="../assets/dc-logo.png" alt="Logo DC">

        <nav>
          <ul>
            <li class="uppercase" v-for="(voice, index) in voices" :key="index" :class="{active:voice.current}">
                <a :href="voice.url">{{ voice.text }} </a>
            </li>
          </ul>
        </nav>
      
  </div>

</template>






<script>
import Voices from '@/data/Voices.js';
export default {
  name: 'Header',
  

  data() {
    return {
            voices: Voices
        }
  }
}
</script>


<style lang="scss" scoped>


.container
{
    display: flex;
}

.header
{
    height: 90px;
    padding: 10px;
}




ul
{
    margin-left: 80px;
    line-height: 70px;
}

li
{
    display: inline-block;
    margin-left: 20px;
    padding-bottom: 4px;
  
    a
    {
        font-size: 14px;  
        color: black;
        font-weight: bold;
        
        
        &:hover
        {
            color: blue;
        }
    }

    &.active 
    {
        border-bottom: 5px solid blue;
        color: blue;

    }
}





</style>
