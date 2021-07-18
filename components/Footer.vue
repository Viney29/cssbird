<template>
  <div :class="$style.footer">
    <p :class="$style.text">Copyright  &copy; 2021 CssBird</p>
  </div>
</template>

<style lang="scss" module>

.footer {
  @include padding($bottom: 'xxs');
  @include blocksize(100%,auto);
  @include text('center');
}

.text {
  color: color('secondary-500');
  @include use-text-style('label');
}

</style>
