<template>
  <svg :viewBox="viewbox">
    <use :href="`#${href}`" />
  </svg>
</template>

<script>
export default {
  props: {
    viewbox: {
      type: String,
      required: true,
    },
    href: {
      type: String,
      required: true,
    },
  },
}
</script>
