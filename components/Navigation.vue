<template>
  <nav role="navigation" aria-label="main navigation" :class="$style.nav">
    <ol :class="$style.ol">
      <li v-for="menu in menuItem" :key="menu.title" :class="$style.li">
        <a :class="$style.link" :href="menu.url" >
          {{ menu.title }}
        </a>
      </li>
    </ol>
    <a :class="$style.resume" href='../assets/resume.pdf' download>resume</a>
  </nav>
</template>

<script>
export default {
  data(){
    return{
      isOpen: false,
      menuItem:[
        {
          title:'About',
          url: '/#about'
        },
        {
          title:'Experience',
          url: '/#jobs'
        },
        {
          title:'Work',
          url: '/#projects'
        },
        {
          title:'Contact',
          url: '/#contact'
        },
      ]
    }
  },
}

</script>

<style lang="scss" module>

.nav {
  @include flex();

  @include below('tablet-large'){
    display: none;
  }
}

.ol {
  @include padding($all: 0);
  @include margin($all: 0);
  @include flex($align-items: center, $justify-content: space-between);

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
