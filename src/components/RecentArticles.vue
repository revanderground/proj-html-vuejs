<template>
  <div id="recent-articles">

    <div class="master-container mt-5 px-4">

        <!-- top-elements -->
        <div class="top-elements d-flex align-items-center justify-content-between py-2">
            <div class="info-critics ">
                <div class="info-title py-1">
                    Recent Articles
                </div>
                <div class="info-subtitle py-2">
                    READ THE LATEST ENTRIES
                </div>
            </div>

            <div>
                <div class="my-button text-center">All Articles</div>
            </div>

        </div>
    </div>

    <!-- Bottom elements with cards -->
    <div class="bottom-elements px-4 d-flex align-items-stretch">

        <div class="left-side ">
            <div class="featured_card">
                <div class="featured-image-box">
                    <img class="featured-image" src="../assets/img/20-Tips-800x471.jpg" alt="">
                
                    <div class="card-title pt-2">
                        20 Creativity Tips
                    </div>

                    <div class="date">
                        By admin | October 24th, 2019<span class="comments"> | Categories: Event, Tips & Tricks </span>
                    </div>

                    <div class="featured-description">
                    Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet.
                    </div>
                
                </div>

           




            </div>

        </div>

        <!-- side-cards -->
        <div class="right-side">
            <div class="card" v-for="(card, index) in sideCards" :key="index">
                <div class="card-box">
                    <div class="card-image-box">
                        <img class="card-image" :src="require('../assets/img/' + card.image)"  >
                    </div>
                    
                    <div class="card-title pt-2">
                        {{card.title}}
                    </div>

                    <div class="date">
                        {{card.date}}, <span class="comments">| {{card.comments}} </span>
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
                    title: `What's On Your Book List`,
                    date: 'October 24th, 2019',
                    comments: '0 Comments',
                    image: 'thumb-13-2x-700x441.jpg'
                },

                {
                    title: `Instanbul travel Guide`,
                    date: 'October 24th, 2019',
                    comments: '0 Comments',
                    image: 'thumb-08-2x-700x441.jpg'
                },



          
            ]
        }
    }    
}
</script>

<style lang="scss" scoped>
@import '../styles/RecentArticles.scss';
@import '../styles/utilities.scss';

</style>