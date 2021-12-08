<template>
  <div :class="$style.block" id="projects">
    <h2 :class="$style.heading">Some Things I've Built</h2>
    <div :class="$style.row">
      <div :class="[$style.item, $style.isReverse]">
        <div :class="$style.content">
          <h4 :class="$style.highlight">Featured Project</h4>
          <h5 :class="$style.name">
             <a :class="$style.projectLink"  target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://rothys.com/">Rothy's</a>
          </h5>
          <div :class="$style.copy">
            <p> Rothy’s is a shoe company using recycled plastic water bottles to create stylish footwear — and improve our planet.</p>
          </div>
          <ul :class="$style.ul">
            <li :class="$style.li">PWA</li>
            <li :class="$style.li">Shopify</li>
            <li :class="$style.li">Optimizely</li>
            <li :class="$style.li">Vuejs</li>
          </ul>
         <a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://rothys.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a>
         <span :class="$style.company">Made at <a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://anatta.io/case-study/rothys">@Anatta</a></span>
        </div>
        <a :class="$style.link"  href="https://rothys.com/" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link">
          <div :class="$style.media"><img :class="$style.image" src="../assets/images/rothys.png" /></div>
        </a>
      </div>
      <div :class="$style.item">
        <div :class="$style.content">
          <h4 :class="$style.highlight">Featured Project</h4>
          <h5 :class="$style.name">
             <a :class="$style.projectLink"  target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://mackweldon.com/">Mackweldon</a>
          </h5>
          <div :class="$style.copy">
            <p>Mack Weldon is a clothing company that’s using premium fabrics and smart design to reinvent men’s basics.</p>
          </div>
          <ul :class="$style.ul">
            <li :class="$style.li">Shopify</li>
            <li :class="$style.li">Optimizely</li>
            <li :class="$style.li">Vuejs</li>
            <li :class="$style.li">web Vitals</li>
          </ul>
         <a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://mackweldon.com/"><span :class="$style.icon"><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 194.818 194.818"><title>External</title><g><path d="M185.818,2.161h-57.04c-4.971,0-9,4.029-9,9s4.029,9,9,9h35.312l-86.3,86.3c-3.515,3.515-3.515,9.213,0,12.728 c1.758,1.757,4.061,2.636,6.364,2.636s4.606-0.879,6.364-2.636l86.3-86.3v35.313c0,4.971,4.029,9,9,9s9-4.029,9-9v-57.04 C194.818,6.19,190.789,2.161,185.818,2.161z"></path><path d="M149,77.201c-4.971,0-9,4.029-9,9v88.456H18v-122h93.778c4.971,0,9-4.029,9-9s-4.029-9-9-9H9c-4.971,0-9,4.029-9,9v140 c0,4.971,4.029,9,9,9h140c4.971,0,9-4.029,9-9V86.201C158,81.23,153.971,77.201,149,77.201z"></path></g></svg></span></a>
         <span :class="$style.company">Made at <a :class="$style.projectLink" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link" href="https://anatta.io/case-study/mackweldon">@Anatta</a></span>
        </div>
        <a :class="$style.link"  href="https://mackweldon.com/" target="_blank" rel="nofollow noopener noreferrer" aria-label="External Link">
          <div :class="$style.media"><img :class="$style.image" src="../assets/images/mw.png" /></div>
        </a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" module>

.block {
  @include padding($top:150px, $bottom: 150px);
  @include margin($left: auto, $right: auto);
  @include max-width(1000px);
}

.heading {
  @include relative();
  @include flex($align-items: center);
  @include margin(10px, 0, 40px, 0);
  @include font-family('primary');

  width: 100%;
  white-space: nowrap;
  font-size: 32px;
  line-height: 42px;
  color: color('primary-200');
  text-transform: capitalize;

  &::before {
    counter-increment: section 1;
    content: "0" counter(section) ".";

    @include relative();
    @include margin($right: 10px);
    @include font-family('secondary');

    color: color('highlight');
    font-weight: normal;
    font-size: 20px;
    bottom: 4px;
  }

  &::after {
    content: "";
    display: block;

    @include relative($top: -5px);
    @include margin($left: 20px);
    @include blocksize(300px, 1px);

    background-color: rgb(45, 57, 82);
  }
}

.row {
  @include flex($direction: column, $align-items: flex-start);
  @include relative();
}

.item {
  @include margin($bottom: 100px);

  display: grid;
  gap: 10px;
  grid-template-columns: repeat(12, 1fr);
  align-items: center;
}

.content {
  @include relative();

  grid-area: 1 / 1 / -1 / 7;
  z-index: 2;
}

.projectLink {
  text-decoration: none;
  color: inherit;

  &:hover {
    color: color('highlight');
  }
}

.link {
  @include relative();

  box-shadow: rgb(2 12 27 / 70%) 0 10px 30px -15px;
  grid-area: 1 / 6 / -1 / -1;
  position: relative;
  z-index: 1;
  background-color: rgb(100, 255, 218);
  border-radius: 4px;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
}

.media{
  display: flex;
  width: 100%;
  max-width: 100%;
  vertical-align: middle;
  border-radius: 3px;
  position: relative;
  mix-blend-mode: multiply;

  &:hover {
    mix-blend-mode: unset;
  }

  img {
    @include blocksize(100%);
  }
}

.highlight {
  @include margin($top: 10px, $bottom: 10px);
  @include font-family('secondary');

  font-size: 13px;
  font-weight: normal;
  color: rgb(100, 255, 218);
  padding-top: 0;
}

.name {
  font-size: 28px;
  line-height: 28px;
  margin: 0 0 20px;
  color: color('primary-200');

  a {
    text-decoration: none;
    color: inherit;

    &:hover {
      color: color('highlight');
    }
  }
}

.copy {
  @include font-family('primary');

  box-shadow: rgb(2 12 27 / 70%) 0 10px 30px -15px;
  transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1) 0s;
  position: relative;
  z-index: 2;
  padding: 25px;
  background-color: rgb(23, 42, 69);
  color: rgb(168, 178, 209);
  font-size: 18px;
  border-radius: 3px;

  p {
    @include margin($bottom: 0);
  }
}

.ul {
  position: relative;
  z-index: 2;
  display: flex;
  flex-wrap: wrap;
  padding: 0;
  margin: 25px 0 10px;
  list-style: none;
}

.li {
  @include relative();
  @include margin($right: 20px, $bottom: 7px);
  @include font-family('secondary');

  font-size: 13px;
  line-height: 17px;
  color: color('primary');
  text-transform: capitalize;
  white-space: nowrap;
}

.icon {

  svg {
    width: 22px;
    height: 22px;
    fill: currentColor;
  }
}


.isReverse {
  .link {
    grid-column: 1 / 8;
  }

  .ul {
    justify-content: flex-end;
  }

  .content {
    grid-column: 7 / -1;
    text-align: right;
  }
}
</style>
