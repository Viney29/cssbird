<template>
  <div :class="$style.block">
    <h1 :class="$style.overline">Hi, my name is</h1>
    <h2 :class="$style.title"> { CssBird }</h2>
    <h3 :class="[$style.title, $style.updateColor]">I am UI Engineer, Biker and Dreamer</h3>
    <div :class="$style.content">
      <p>I am passionate about building websites that improves the user experience. I specialize in creating e-commerce websites for clients ranging from individuals and small-businesses all the way to large enterprise corporations</p>
    </div>
    <a href="mailto:viney.bishnoi@gmail.com" :class="$style.cta" rel="nofollow noopener noreferrer">get in touch</a>
  </div>
</template>

<style lang="scss" module>

.block {
  @include padding($top:150px, $right: 20px, $bottom: 45px, $left: 20px);
  @include margin($left: auto, $right: auto);

  width: 100%;

  @include above('tablet'){
    @include padding($top:150px, $bottom: 75px);
  }

  @include above('tablet-large'){
    @include padding(200px,0, 150px,0);
    @include max-width(1000px);
  }
}

.overline {
  @include margin(0, 0, 20px, 3px);
  @include use-text-style('overline');

  color: color('highlight');
}

.title {
  @include font-family('primary');

  font-size: rem(32px);
  line-height: 1.1;
  font-weight: 600;
  color: color('primary-200');

  @include above('tablet'){
    font-size: rem(60px);
  }

  @include above('tablet-large'){
    font-size: rem(80px);
  }
}

.updateColor {
  @include margin($bottom: 10px);

  color: color('primary');
}

.content {
  @include margin($top: 25px);
  @include max-width(500px);
  @include use-text-style('copy');
}

.cta {
  @include padding(1.25rem, 1.75rem, 1.25rem, 1.75rem);
  @include margin($top: 50px);
  @include use-text-style('button');

  display: inline-flex;
  color: color('highlight');
  background-color: transparent;
  border: 1px solid color('highlight');
  border-radius: 3px;
  text-decoration: none;
  text-transform: capitalize;
  cursor: pointer;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
  margin-top: 50px;

  &:hover {
    background-color: rgba(100, 255, 218, 0.07);
  }
}
</style>
