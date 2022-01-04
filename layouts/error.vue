<template>
  <div :class="$style.error">
    <h1>404 Page</h1>
  </div>
</template>

<style lang="scss" module>

@include import-webfonts();

html {
  @include font-family('primary');

  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  overflow-x: hidden;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

body {
  background-color: color('primary-bg');
  color: color('primary');
  overflow-x: hidden;
  scroll-behavior: smooth;

  @include font-family('primary');
}

p {
  @include margin(0,0,15px,0);
}

.error {
  min-height: calc(100vh - 131px);
  @include flex($align-items: center, $justify-content: center);

  @include above('tablet'){
    min-height: calc(100vh - 90px);
  }
}

</style>
