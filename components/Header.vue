<template>
  <header :class="$style.header">
    <logo :class="$style.logo" />
    <Navigation />
    <sideMenu />
  </header>
</template>

<style lang="scss" module>

.header {
  @include padding($left: 20px, $right: 20px);
  @include flex($justify-content: space-between, $align-items: center);
  @include blocksize(100%, 100px);

  position: sticky;
  top: 0;
  z-index: 11;

  @include above('tablet-large'){
     @include padding($left: 50px, $right: 50px);
  }
}

.center {
  @include flex();
}

</style>
