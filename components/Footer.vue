<template>
  <div :class="$style.footer">
    <p :class="$style.text">
    <a :class="$style.link"  href="https://github.com/Viney29" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link"> Designed &amp; Developed by Viney Bishnoi </a>
    <span :class="$style.copyright">Copyright &copy; 2021 CssBird</span>
    </p>
  </div>
</template>

<style lang="scss" module>

.footer {
  @include padding($all: 15px);
  @include flex($direction: column, $align-items: center, $justify-content: center);
  @include blocksize(100%,auto);
  @include text('center');

  background-color: rgb(2, 12, 27);
  min-height: 70px;
  color: rgb(136, 146, 176);
}

.text {
  @include padding($all: 10px);
  @include margin($bottom: 0);
  @include use-text-style('label');

  color: color('primary-100');
}

.link {
  text-decoration: none;
  color: color('primary-100');

  &:hover {
    color: color('highlight');
  }
}

.copyright {
  @include margin($top: 10px);

  display: block;
  font-size: 12px;
  line-height: 16px;
  color: color('primary-100');
  text-align: center;
}

</style>
