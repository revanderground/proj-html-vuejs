<template>
    <div id="Events">
        <div class="container-events">

            <div class="events-details text-center pt-3">
                <h2 class="section-title">
                    Upcoming Events
                </h2>

                 <h4 class="section-subtitle py-1 pb-3">
                   MEET THE AUTHOR IN PERSON
                 </h4>

            </div>

            <div class="cards-box d-flex flex-wrap text-center mt-4">
                <EventsCard class="event-card col-4 px-3" v-for="(card, index) in eventCards" :key="index" :singleCard="card" />

            </div>
         

        </div>
    
    </div>

</template>

<script>
import EventsCard from "../components/EventsCard.vue";

export default {

    components:{
        EventsCard,
    },

    data: function(){
        return {
            eventCards: [
                {
                    title: 'Chicago Book Signing',
                    description: 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.',
                    image: 'event-05-600x359.jpg'
                },

                {
                    title: 'Meet & Greet With Amanda',
                    description: 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Praesent sapien massa, convallis a pellentesque nec, egestas.',
                    image: 'event-04-600x359.jpg'
                },

                {
                    title: 'Open Book: Dialogues',
                    description: 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.',
                    image: 'event-07-600x359.jpg'
                },

               



          
            ]
        }
    }    
}
</script>

<style lang="scss" scoped>
@import '../styles/Events.scss';
@import '../styles/utilities.scss';

</style>