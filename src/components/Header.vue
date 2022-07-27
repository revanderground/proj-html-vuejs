<template>
    <header>
        <div class="container-fluid">
            <div class="jumbotron">
                <div class="topbar-container d-flex justify-content-between">
                    <div class="box-logo">
                        <img class="logo" src="../assets/img/author-logo-round-small.png" alt="logo">
                    </div>

                    <nav class="top-navbar">
                        <ul class="navbar-list d-flex justify-content-end ">
                            <li class="list-element text-center mx-3 py-2" v-for="(element, index) in navbarElements" :key="index" :class="{ active: element.current}">
                            <a :href="element.url">{{element.text}}</a>
                            </li>
                            <li class="list-element text-center mx-3 py-2">
                             <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
                            </li>
                            
                        </ul>

                    </nav>


                </div>

                
                <div class="content-box row">
                    <div class="left-box col-7">

                        <div class="jumbotron-text">
                            <div class="jumbotron-name">
                                Damon Vaughn
                            </div>
                            <div class="jumbotron-description py-3">
                                Best-selling author and the most influential pubblic intellectual in the western world right now.
                            </div>
                            <div class="jumbotron-author">
                                - The New York Times
                            </div>

                            <div class="buttons-carousel">
                                <button ></button>
                            </div>

                        </div>
                       

                    </div>

                    <div class="right-box col-5">
                        <div class="widget-box p-5">
                            <div class="widget d-flex">
                                <div class="widget-img-box">
                                    <img class="widget-img" src="../assets/img/book-widget.png" alt="">
                                </div>
                                <div class="widget-text">
                                    
                                    <div class="widget-title py-2">
                                        Latest Book Release
                                    </div>
                                    
                                    <div class="widget-subtitle py-1">
                                        D. VAUGHN AUTOBIOGRAPHY
                                    </div>
                                    
                                    <div class="widget-description py-2">
                                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit sit voluptatum aliquam ipsam optio, nisi saepe, eius non quo.
                                    </div>

                                </div>
                            
                            </div>
                            
                            




                        

                        </div>
                      

                    </div>

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

    @import '../styles/style.scss'; 
    @import '../styles/viarables.scss';
    @import '../styles/Header.scss'
 
    

</style>