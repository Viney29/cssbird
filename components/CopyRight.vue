<template functional>
  <div :class="$style.copyright"><span :class="$style.text">Copyright &copy; {{ props.text }}</span></div>
</template>

<script>
export default {
  props:{
    text: {
      type:String,
      default: "2021 CssBird"
    }
  }
}
</script>
