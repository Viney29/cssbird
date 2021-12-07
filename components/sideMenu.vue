<template>
  <div :class="$style.mobileMenu">
      <span @click="isActive" :class="[$style.menuIcon, {[$style.isOpen] : isOpen}]">
      <span :class="$style.line"></span>
      <span :class="$style.line"></span>
      <span :class="$style.line"></span>
    </span>
    <div :class="[$style.sidebar, {[$style.isOpen] : isOpen}]">
      <aside :class="$style.sidebarMenu">
        <nav :class="$style.nav">
          <ol :class="$style.ol">
            <li v-for="menu in menuItem" :key="menu.title" :class="$style.li">
              <nuxt-link :class="$style.link" :to="menu.url" >
                {{ menu.title }}
              </nuxt-link>
            </li>
          </ol>
        <a :class="$style.resume" href='../assets/resume.pdf' download>resume</a>
      </nav>
      </aside>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      isOpen: false,
      menuItem:[
        {
          title:'About',
          url: '#about'
        },
        {
          title:'Experience',
          url: '#jobs'
        },
        {
          title:'Work',
          url: '#projects'
        },
        {
          title:'Contact',
          url: '#contact'
        },
      ]
    }
  },
  methods:{
    isActive: function() {
      this.isOpen = !this.isOpen;
    },
  }
}

</script>

<style lang="scss" module>

.mobileMenu {
  @include above('tablet-large'){
    display: none;
  }
}

.line {
  display: block;

  @include blocksize(100% , 2px);

  background-color: color('highlight');
  transition:  all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;

  &:nth-child(even){
    @include margin($top:10px, $bottom: 10px);

    width: 85%;
    margin-left: 15%;
  }
}

.menuIcon {
  @include absolute($top: 31px, $right: 23px);
  @include blocksize(32px);

  z-index: 9999;
  color: color('primary');;
  display: block;
  cursor: pointer;

  &.isOpen {
    overflow: hidden;

    .line {
      &:first-child {
        transform: translateY(12px) rotate(45deg);
      }
      &:nth-child(2) {
        opacity: 0;
      }
      &:last-child {
        transform: translateY(-12px) rotate(-45deg);
      }
    }
  }

  @include above('tablet-large'){
    display: none;
  }
}

.sidebar {
  @include fixed(0,0,0);
  @include blocksize(100%, 100vh);

  z-index: 10;
  outline: 0;
  transform: translateX(100%);
  visibility: hidden;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;

  &.isOpen {
    visibility: visible;
    transform: translateX(0%);
  }
}

.sidebarMenu {
  @include flex($direction: column, $align-items: center, $justify-content: center);
  @include padding($all: 50px);
  @include blocksize(75vw, 100%);
  @include relative();
  @include font-family('secondary');

  background-color: rgb(23, 42, 69);
  z-index: 99;
  right: 0;
  margin-left: auto;
  box-shadow: rgb(2 12 27 / 70%) -10px 0 30px -15px;

  @include above('tablet'){
    width: 50vw;
  }
}

.nav {
  @include flex($direction: column, $justify-content: space-between, $align-items: center);

  width: 100%;
  text-align: center;
  color: rgb(204, 214, 246);
}

.ol {
  @include padding($all: 0);
  @include margin($all: 0);
  @include flex($direction: column, $align-items: center, $justify-content: space-between);

  list-style: none;

  @include below('tablet-large'){
     @include margin($bottom: 20px);
  }
}

.li {
  @include relative();
  @include margin($left: 10px, $right: 10px);
  @include use-text-style('navigation');

  counter-increment: item 1;

  @include below('tablet-large'){
    @include update-text-style('subtitle');
  }

  &::before {
    content: "0" counter(item) ".";
    color: color('highlight');

    @include text('right');

    @include below('tablet-large'){
      position: absolute;
      left: 0;
    }
  }

  @include below('tablet-large'){
    min-width: 200px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}

.link {
  @include relative();
  @include padding(12px, 10px, 12px, 10px);

  color: color('primary-200');
  display: inline-block;
  text-decoration: none;
  cursor: pointer;

  &:hover {
    color: color('highlight');
  }
}

.resume {
  @include padding(0.75rem, 1rem,0.75rem, 1rem );
  @include use-text-style('navigation');

  text-decoration: none;
  background-color: transparent;
  border-radius: 3px;
  border: 1px solid color('highlight');
  color: color('highlight');
  text-transform: capitalize;

  @include below('tablet-large'){
    @include padding(0.75rem, 2rem,0.75rem, 2rem );
  }
}

</style>
