<template>
  <main>

     <SectionHero/>

  </main>
</template>

<script>
import SectionHero from '../sections/SectionHero.vue';
export default {
    name: "BaseMain",
    components:{
    SectionHero,
}
}
</script>

<style lang="scss" scoped>
// main{
//     // background-color: var(--secondary-color);
//     // width: 100%;

//     // & .container p{
//     //     padding: 3rem 0;
//     //     color: white;
//     //     font-size: 2.5rem;
//     // }
// }
</style>