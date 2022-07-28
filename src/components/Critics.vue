<template>
  <div class="critics-section mb-5">

    <div class="master-container mt-5 px-4">

        <!-- top-elements -->
        <div class="top-elements d-flex align-items-center justify-content-between py-2">
            <div class="info-critics ">
                <div class="info-title py-1">
                    What The Critics Say
                </div>
                <div class="info-subtitle py-2">
                    TESTIMONIALS FROM AROUND THE WORLD
                </div>
            </div>

            <div>
                <div class="my-button text-center">Read All Testimonials</div>
            </div>

        </div>
    </div>

    <!-- Bottom elements with cards -->
    <div class="bottom-elements px-4 d-flex">

        <div class="left-side ">
            <div class="featured_card">
                <div class="featured_card-text">
                    <h3 class="featured_card-title pb-4">
                        Best Author Of His Generation
                    </h3>

                   <h3 class="featured_card-subtitle pb-3 pt-4">
                        This book will change your perspective on life
                    </h3>

                    <div class="featured_card-description">
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptate in aut quasi aliquid asperiores, eaque nemo quaerat illum iusto omnis dolorum maxime quo nostrum sunt porro suscipit facilis reprehenderit deserunt?</p>
                        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptas delectus, maiores explicabo sequi neque quas nemo, id natus facilis fuga doloremque odit reiciendis praesentium nobis dolore inventore quidem laborum tenetur.</p>
                    </div>

                    <div class="featured_card-info_author d-flex align-items-center">
                        <div class="company-logo-box">
                            <img class="featured_company-logo" src="../assets/img/nytimes-logo-white-xsmall.png" alt="">
                        </div>

                        <div class="featured_author px-3 py-4">
                            Justine Kilpatrick, <span class="featured_company"> The New York Times </span>
                        </div>

                    </div>

                </div>

            </div>

        </div>

        <!-- side-cards -->
        <div class="right-side">
            <div class="card pb-2" v-for="(card, index) in sideCards" :key="index">
                <div class="card-text text-center">
                    <h3 class="card-title">
                        {{card.title}}
                    </h3>

                    <div class="card-description">
                        {{card.description}}
                    </div>
                </div>    

                <div class="card-info_author d-flex align-items-center">
                    <div class="company-logo-box">
                        <img class="company-logo" :src="require('../assets/img/' + card.logo)"  >
                    </div>

                    <div class="author px-3 pt-3 pb-2">
                        {{card.author}}, <span class="company"> {{card.company}} </span>
                    </div>

                </div>

            </div>

             

        </div>

    </div>
</div>


</template>

<script>


export default {
      data: function(){
        return {
            sideCards: [
                {
                    title: 'A True Masterpiece, Bravo!',
                    description: 'Nulla quis lorem ut libero malesuada feugiat. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus suscipit tortor eget felis porttitor volutpat. Nulla quis lorem ut libero malesuada feug at.',
                    author: 'Gerald Hendley',
                    company: 'The Guardian',
                    logo: 'theguardian-xsmall.png'
                },

                {
                    title: 'A Unique View On The World',
                    description: 'Donec sollicitudin molestie malesuada. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui. Nulla quis lorem ut libero malesuada feugiat. Vestibulum ac diam sit amet.',
                    author: 'Mary Maxey',
                    company: 'The Globe And Mail',
                    logo: 'globe-xsmall.png'
                },



          
            ]
        }
    }    
}
</script>

<style lang="scss" scoped>
@import '../styles/Critics.scss';
@import '../styles/utilities.scss';

</style>