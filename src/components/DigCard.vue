<template>
    <div>
        
        <div class="wrapper-cards">

            <div class="imgcard-box">
            <img class="card-image" :src="require('../assets/img/' + singleDigCard.image)" alt="event-image">
            
            <div class="card-info">

                <div class="card-title">
                    {{singleDigCard.title}}
                </div>

                <div class="breakline"> 
                </div>

                <div class="card-description">
                    {{singleDigCard.description}}
                </div>


            </div>
            
            </div>

   

        </div>

        
    </div>
  
</template>

<script>
export default {
    props: {
        singleDigCard: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../styles/Digdeeper.scss';
@import '../styles/utilities.scss';

</style>