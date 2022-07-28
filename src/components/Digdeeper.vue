<template>
    <div id="digdeeper">
 <div class="container-digs">

            <div class="digs-details text-center pt-3">
                <h2 class="section-title">
                    Dig A Little Deeper Into Damon Vaughn
                </h2>

                 <h4 class="section-subtitle py-1 pb-3">
                   FIND OUT MORE ABOUT THE AUTHOR HIMSELF
                 </h4>

            </div>

            <div class="cards-box d-flex flex-wrap text-center mt-4">
                <DigCard class="event-card col-4 px-3" v-for="(card, index) in digCards" :key="index" :singleDigCard="card" />

            </div>
         

        </div>
    
    </div>

</template>

<script>
import DigCard from "../components/DigCard.vue";

export default {

    components:{
        DigCard,
    },

    data: function(){
        return {
            digCards: [
                {
                    title: 'About Me',
                    description: 'Vestibulum ante ipsum primis',
                    image: 'box-1.jpg'
                },

                {
                    title: 'My Latest Book',
                    description: 'Vestibulum ante ipsum primis',
                    image: 'box-4.jpg'
                },

                {
                    title: 'Book Signing',
                    description: 'Vestibulum ante ipsum primis',
                    image: 'box-3.jpg'
                },

               



          
            ]
        }
    }    
}
</script>

<style lang="scss" scoped>
@import '../styles/Digdeeper.scss';
@import '../styles/utilities.scss'

</style>