<template>

    <main>
        
        <div class="main-top">
            <div class="container">
                <h2>--> Contents goes here</h2>
            </div>
        </div>
        

        <div class="main-bottom">
            <div class="container">
                <nav>
                    <ul>
                      <li class="uppercase" v-for="(item, index) in items" :key="index"><a :href="item.url">{{ item.text }} </a></li>
                    </ul>
                </nav>
            </div>
        </div>

    </main>

    
</template>

<script>
export default {
  name: 'Main',
  data() {
    return {
            items: [
                {
                    text: 'Digital Comics',
                    url: '#',
                    img:  'buy-comics',                  
                },
                {
                    text: 'DC Merchandise',
                    url: '#',
                    img: 'buy-comics',              
                },
                {
                    text: 'Subscription',
                    url: '#',
                    img: 'buy-comics',                   
                },
                {
                    text: 'Comic Shop Locator',
                    url: '#',
                    img: 'buy-comics',                   
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                    img: 'buy-comics',                    
                }
            ]
        }
  }
}
</script>

<style lang="scss" scoped>

main
{
   
    
    .main-top
    {
        background-color: black;
        height: 100px;
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
        }
        
    }


}





</style>
