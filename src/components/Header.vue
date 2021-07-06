<template>

  <div class="container">
      
        <img src="../assets/dc-logo.png" alt="Logo DC">

        <nav>
          <ul>
            <li class="uppercase" v-for="(voice, index) in voices" :key="index" :class="{active:voice.current}"><a :href="voice.url">{{ voice.text }} </a></li>
          </ul>
        </nav>
      
  </div>

</template>






<script>
export default {
  name: 'Header',

  data() {
    return {
            voices: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false
                },
                {
                    text: 'Tv',
                    url: '#',
                    current: false
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false
                },
                {
                    text: 'News',
                    url: '#',
                    current: false
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false
                },
            ]
        }
  }
}
</script>


<style lang="scss" scoped>


.container
{
    display: flex;
}


img
{
    width: 80px;
  
}

ul
{
    margin-left: 70px;
    margin-top: 18px;
}

li
{
    display: inline-block;
    padding: 10px;
  
    a
    {
        font-size: 14px;  
        
        &:hover
        {
            color: blue;
        }
    }

    &.active 
    {
        border-bottom: 2px solid blue;
        // padding: 20px;
    }
}





</style>
