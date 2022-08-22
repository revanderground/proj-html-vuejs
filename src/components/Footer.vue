<template>
    <footer id="footer">
        <div class="container-fluid">
            <div class="jumbotron">
                <div class="container">

                    <ul class="section-list d-flex ">

                        <li class="section-logo col-2">
                            <div class="logo-img">
                            <img class="logo" src="../assets/img/author-logo-round.png" alt="logo">
                            </div>

                        </li>
                        


                        <li class="about-me-section col-3">
                            <div class="footer-title">ABOUT ME</div>
                            <div class="footer-text">
                                Vivamus suscipit tortor eget felis porttitor volutpat. Nulla quis lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis porttitor volutpat.
                            </div>

                        </li>

                        <li class="links-section col-3">
                            <div class="footer-title px-4">USEFUL LINKS</div>
                                <ul class="footer-text white">
                                    <li class="list-element" v-for="(element, index) in footerCenterElements" :key="index" >
                                        <i class="fa-solid fa-angle-right px-1"></i> <a class="link-footer-center" :href="element.url">{{element.text}}</a>
                                    </li>
                           
                            
                                </ul>

                        </li>

                        <li class="contact-info col-4">
                            <div class="footer-title">CONTACT INFO</div>
                            <div class="footer-text">63 E. Studebaker Street Bolingbrook, IL 60440</div>
                            <div class="footer-text">Phone: (800) 000-0000</div>
                            <div class="footer-text">Mobile: (800) 000-0000</div>
                            <div class="footer-text">Email: <a class="link-text" href="mailto:info@your-company.com">info@your-company.com</a></div>
                            <div class="social-logos d-flex ">
                                <div class="logo-social"><i class="logo-social-icon fa-brands fa-facebook-f"></i></div>
                                <div class="logo-social"><i class="logo-social-icon fa-brands fa-twitter"></i></div>
                                <div class="logo-social"><i class="logo-social-icon fa-brands fa-instagram"></i></div>
                                <div class="logo-social"><i class="logo-social-icon fa-brands fa-youtube"></i></div>
                                <div class="logo-social"><i class="logo-social-icon fa-brands fa-linkedin-in"></i></div>
                                

                            
                            
                            </div>

                        </li>


                    </ul>

                    <div class="footer-text text-center copyright-text white">© Copyright 2012 - 2022 | Avada Theme by <a class="link-text grey" href="http://theme-fusion.com/">ThemeFusion</a> | All Rights Reserved | Powered by <a class="link-text grey" href="http://wordpress.org/">Wordpress</a></div>
                        

                </div>
                
                

            </div>

        </div>

    </footer>
  
</template>

<script>
export default {
      data: function(){
        return {
            footerCenterElements: [
                {
                    text: 'Latest Books',
                    url: '#',
                    
                },
                {
                    text: 'Upcoming Events',
                    url: '#',
                   
                },
                {
                    text: 'Recent Articles',
                    url: '#',
                    
                },
                {
                    text: 'Business Enquires',
                    url: '#',
                    
                },
                {
                    text: 'Visit My Foundation',
                    url: '#',
                    
                },      
          
            ]
        }
    }    
}


</script>

<style lang="scss" scoped>
    @import '../styles/variables.scss';
    @import '../styles/Footer.scss'
 
    

</style>