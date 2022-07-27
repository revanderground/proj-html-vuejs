<template>

  <main>
    <MoreAbout />
    <Audiobook />
    <Critics />
    <Events />
    <Newsletter />
    <Digdeeper />
    <RecentArticles />

  </main> 

</template>

<script>
import MoreAbout from './MoreAbout.vue';
import Audiobook from './Audiobook.vue';
import Critics from './Critics.vue';
import Events from './Events.vue';
import Newsletter from './Newsletter.vue';
import Digdeeper from './Digdeeper.vue';
import RecentArticles from './RecentArticles.vue';


export default {
    components: {
        MoreAbout,
        Audiobook,
        Critics,
        Events,
        Newsletter,
        Digdeeper,
        RecentArticles
    }
}
</script>

<style>

</style>