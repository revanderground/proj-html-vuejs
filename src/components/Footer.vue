<template>
    <header id="header">
        <div class="container-fluid">
            <div class="jumbotron">
                
                

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
    @import '../styles/viarables.scss';
    @import '../styles/Footer.scss'
 
    

</style>