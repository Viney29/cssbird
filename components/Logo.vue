<template>
  <span :class="$style.logo"><nuxt-link to="/">{ CssBird }</nuxt-link></span>
</template>

<style lang="scss" module>
.logo {
  color: color('highlight');
  font-size: 24px;
  text-decoration: none;

  a {
    text-decoration: none;
    color: inherit;
  }
}
</style>
