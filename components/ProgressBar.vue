<template>
  <div :class="$style.progressBar">
    <span :class="$style.label">0%</span>
    <span :class="$style.progress"><span :class="$style.filled"></span></span>
    <span :class="$style.label">100%</span>
  </div>
</template>

<script>
export default {
  props:{
    percentage:{
      type: Number,
      default: 70
    }
  }
}
</script>

<style lang="scss" module>

.progressBar {
  @include margin($top: 's');
  @include flex($align-items: center, $justify-content: space-between);
  @include blocksize(100%, 20px);

  flex-wrap: wrap;
}

.progress {
  @include relative();
  @include blocksize(100%, 20px);

  order: 1;
  background-color: #f2f2f2;
}

.filled {
  @include blocksize(65%, 100%);
  @include absolute($left: 0);

  background: linear-gradient(99deg,color('highlight'),color('highlight-100'),color('highlight'));
  background-size: 400% 400%;
  animation: grad 3s ease-in-out infinite;
}

.label {
  order: 2;
  @include margin($top: 'base');
  @include use-text-style('label');
}
</style>
