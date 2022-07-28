<template>
    <div>
        
        <div class="wrapper-cards">

            <div class="imgcard-box">
            <img class="card-image" :src="require('../assets/img/' + singleCard.image)" alt="event-image">
            </div>

            <div class="card-info">

                <div class="card-title">
                    {{singleCard.title}}
                </div>

                <div class="card-description">
                    {{singleCard.description}}
                </div>


            </div>
   

        </div>

        
    </div>
  
</template>

<script>
export default {
    props: {
        singleCard: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../styles/Events.scss';
@import '../styles/utilities.scss';

</style>