<template>
  <header :class="[$style.header, (scrolled ? $style.isUnpinned : $style.isPinned )]" @scroll="handleScroll">
    <logo :class="$style.logo" />
    <Navigation />
    <sideMenu />
  </header>
</template>

<script>
export default {
  data(){
    return{
      limitPosition: 500,
      scrolled: false,
      lastPosition: 0
    }
  },
  methods: {
    handleScroll() {
      if (this.lastPosition < window.scrollY && this.limitPosition < window.scrollY) {
        this.scrolled = true;
        // move up!
      }

      if (this.lastPosition > window.scrollY) {
        this.scrolled = false;
        // move down
      }

      this.lastPosition = window.scrollY;
      // this.scrolled = window.scrollY > 250;
    }
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  }
}
</script>


<style lang="scss" module>

.header {
  @include fixed();
  @include padding($left: 20px, $right: 20px);
  @include flex($justify-content: space-between, $align-items: center);
  @include blocksize(100%, 100px);

  z-index: 11;
  will-change: transform;
  transition: transform 200ms linear;


  @include above('tablet-large'){
    @include padding($left: 50px, $right: 50px);
  }

  &.isPinned {
    transform: translateY(0%);
    background-color: rgb(10, 25, 47);
    box-shadow: rgb(2 12 27 / 70%) 0 10px 30px -10px;
  }

  &.isUnpinned {
    transform: translateY(-100%);
  }
}

.center {
  @include flex();
}

</style>
