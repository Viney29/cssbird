<template>
  <div :class="$style.main">
    <div :class="$style.wrapper">
      <h1 :class="$style.heading">Under <br> Construction</h1>
      <h3 :class="$style.subheading">Site nearly ready</h3>
      <progress-bar />
    </div>
  </div>
</template>


<style lang="scss" module>
.main {
  @include flex($align-items: center, $justify-content: center);

  background-color: #ece93f;
  min-height: calc(100vh - 60px);
}

.wrapper {
  @include flex($direction: column, $justify-content: center);
}

.heading {
  @include use-text-style('heading-2');
  @include text('center');

  color:color('secondary-500');
  text-transform: uppercase;

  @include above('tablet'){
    @include update-text-style('heading');
  }
}

.subheading {
  @include use-text-style('title');
  @include text('center');

  color:color('secondary-500');
  text-transform: uppercase;

  @include above('tablet'){
    @include update-text-style('subheading');
  }
}

</style>
