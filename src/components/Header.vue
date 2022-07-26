<template>
    <header>
        <div class="container-fluid">
            <div class="jumbotron">
                <div class="topbar-container d-flex justify-content-between">
                    <div class="box-logo">
                        <img class="logo" src="../assets/img/author-logo-round-small.png" alt="logo">
                    </div>

                    <nav class="navbar">
                        <ul class="d-flex justify-content-end">
                            <li class="text-center px-3" v-for="(element, index) in navbarElements" :key="index" :class="{ active: element.current}">
                            <a :href="element.url">{{element.text}}</a>
                            </li>
                            
                        </ul>

                    </nav>
                </div>
                

            </div>

        </div>

    </header>
  
</template>

<script>
export default {
      data: function(){
        return {
            navbarElements: [
                {
                    text: 'Home',
                    url: '#',
                    current: true,
                },
                {
                    text: 'About Me',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Testimonials',
                    url: '#',
                    current: false,
                },
                {
                    text: 'My Blog',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Meetups',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shops',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Contact Me',
                    url: '#',
                    current: false,
                },
          
            ]
        }
    }    
}


</script>

<style lang="scss" scoped>

    .jumbotron{
        @import '../styles/style.scss'; 
        @import '~bootstrap/scss/bootstrap.scss';       
        
        background-image: linear-gradient(0deg, rgba(0,0,0,0.7375992633381477) 0%, rgba(0,0,0,0.5163107479319853) 55%, rgba(119,119,119,0.21098861908044464) 100%), url('../assets/img/hero-07-2x.jpg');
        background-position: center center;
        background-repeat: no-repeat;
        border-width: 0px;
        border-style: solid;
        background-size: cover;
        height: 100vh;

        .topbar-container{
            max-width: 88%;
            border: 1px solid red;
            height: 100px;
            margin: 0 auto;
 
        }
    }
    
    .logo{
        height: 130px;
    }

    li{
        list-style-type: none;
    }
    

</style>