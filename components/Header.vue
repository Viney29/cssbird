<template>
  <div :class="$style.header">
    <logo :class="$style.logo" />
    <div :class="$style.center">
      <Navigation />
    </div>
    <div :class="$style.right">
    </div>
  </div>
</template>

<style lang="scss" module>

.header {
  @include flex();
}

.center {
  @include flex();
}

</style>
