<template>
  <div :class="$style.block">
    <hero />
    <about />
    <experience />
    <work />
    <projects />
    <contact />
  </div>
</template>

<script>
import hero from './-hero.vue';
import about from './-about.vue';
import Experience from './-experience.vue';
import work from './-work.vue';
import projects from './-projects.vue';
import contact from './-contact.vue';
export default {
  components:{
    hero,
    about,
    Experience,
    work,
    projects,
    contact
  }
}
</script>

<style lang="scss" module>

.block {
  @include margin($left: auto, $right: auto);

  width: 100%;
  max-width: 1600px;
  min-height: 100vh;
  counter-reset: section 0;
}

</style>
