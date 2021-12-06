<template>
  <div orientation="right" :class="$style.right">
    <div :class="$style.wrapper">
      <a href="mailto:viney.bishnoi@gmail.com" target="_blank" rel="nofollow noopener noreferrer" aria-label="Twitter" :class="$style.link">viney.bishnoi@gmail.com</a>
    </div>
  </div>
</template>

<style lang="scss" module>

.right {
  @include fixed($right: 40px, $bottom: 0, $left: auto);

  width: 40px;
  z-index: 10;
  color: rgb(168, 178, 209);
}

.wrapper {
  @include relative();
  @include flex($direction: column, $align-items: center);

  &::after {
    content: "";
    display: block;
    @include margin(0, auto, 0, auto);
    @include blocksize(1px, 90px);

    background-color: rgb(168, 178, 209);
  }
}

.link {
  @include relative();
  @include padding($all: 10px);
  @include margin(20px, auto, 20px, auto);

  display: inline-block;

  @include font-family('secondary');

  font-size: 12px;
  letter-spacing: 0.1em;
  color: inherit;
  text-decoration: none;
  text-decoration-skip-ink: auto;
  cursor: pointer;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
  writing-mode: vertical-rl;


  &:hover,
  &:focus {
    transform: translateY(-3px);
    color: color('highlight')
  }
}
</style>
