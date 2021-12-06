<template>
  <div :class="$style.sidebar">
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
}

</script>

<style lang="scss" module>

.sidebar {
  @include fixed(0,0,0);
  @include blocksize(100%, 100vh);

  z-index: 10;
  outline: 0;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
  transform: translateX(0);
  visibility: visible;


  @include above('tablet-large'){
   display: none;
  }
}

.sidebarMenu {
  @include flex($direction: column, $align-items: center, $justify-content: center);
  @include padding($all: 50px);
  @include blocksize(50vw, 100%);
  @include relative();
  @include font-family('secondary');

  background-color: rgb(23, 42, 69);
  z-index: 99;
  right: 0;
  margin-left: auto;
  box-shadow: rgb(2 12 27 / 70%) -10px 0 30px -15px;
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
}

.li {
  @include relative();
  @include margin($left: 10px, $right: 10px);
  @include use-text-style('navigation');

  counter-increment: item 1;

  &::before {
    content: "0" counter(item) ".";
    color: color('highlight');

    @include text('right');
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
  padding: 0.75rem 1rem;
  @include use-text-style('navigation');

  text-decoration: none;
  background-color: transparent;
  border-radius: 3px;
  border: 1px solid color('highlight');
  color: color('highlight');
  text-transform: capitalize;
}

</style>
