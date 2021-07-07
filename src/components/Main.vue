<template>

    <main>
        
        <div class="main-top">
            <div class="container">
                <Series
                v-for="(serie,index) in series" 
                :key="index"
                :prod="serie"/>

                
            </div>
        </div>
        

        <div class="main-bottom">
            <div class="container">
                <nav>
                    <ul>
                        <li class="uppercase" v-for="(item, index) in items" :key="index">
                            <a href="#">
                                <img class="image" :src="item.img" alt="item.text">
                                {{item.text}} 
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>

    </main>

    
</template>

<script>
import Series from '@/components/Series.vue'
import Items from '@/data/Items.js'
import CurrentSeries from '@/data/CurrentSeries.js'

export default {
  name: 'Main',

  components: {
      Series
  },

  data() {
    return {
            
            items: Items,
            series: CurrentSeries
        }
  },

}
</script>

<style lang="scss" scoped>

main
{
   
    
    .main-top
    {
        background-color: #1c1c1c;
        height: 500px;
        padding: 20px
    }

    .main-bottom
    {
        background-color: #0282f9;
        height: 120px;
        
    }

    h2
    {
        color: white;
        line-height: 100px;
    }

    ul
    {
        display: flex;
        justify-content: space-between;
        line-height: 120px;
        

        a
        {
            color: white;
            font-size: 14px;
        }
        
    }

    .image
    {
        width: 40%;
        padding: 10px;
        vertical-align: middle;
    }
}





</style>
