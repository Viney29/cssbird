<template>
  <div :class="$style.bar"><span :class="$style.text">This Website is in Beta. Cssbird is working tirelessly to finish it soon !! </span></div>
</template>

<style lang="scss" module>

.bar {
  @include flex($align-items: center, $justify-content: center);
  @include blocksize(100%, 30px);
  // @include use-text-style('copy-small');

  color: color('highlight');
  background-color: color('secondary-500');

  &:hover {
    cursor: pointer;
  }

}

.text{
  @include padding($left: 100%);

  white-space: nowrap;
  display: inline-block;

  @include font-family('secondary');

  font-size: 12px;
  line-height: 16px;
  font-weight: 600;
  letter-spacing: 2px;
  will-change: transform;
  animation: marquee 20s linear infinite;
  z-index: 2;

  &:hover {
    animation-play-state: paused;
  }
}
</style>
