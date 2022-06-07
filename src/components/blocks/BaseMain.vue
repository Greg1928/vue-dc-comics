<template>
  <main>
    <SectionHero/>
    <SectionThumb/>
  </main>
</template>

<script>
import SectionHero from '../sections/SectionHero.vue';
import SectionThumb from '../sections/SectionThumb.vue';

export default {
    name: "BaseMain",
    components:{
        SectionHero,
        SectionThumb,
}
}
</script>

<style>
</style>